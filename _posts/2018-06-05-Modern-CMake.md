This is how I use CMake in my projects.

## General Idea

The new CMake paradigm introduced with version 3.0 is about __Targets and Properties__.

* **Modular**

Modular means that there are clear dependencies and that replacing a component is doable and easy as long as the API to the rest of the system is still fulfilled.

* **Encapsulated**

The focus should be kept at the target level without any concerns about the whole system.

* **Transitive**

Target flags are handled by CMake and propagated to depending targets.

## Patterns

I declare libraries as such:

```
add_library(mylib
            src/file1.cpp
            src/file2.cpp)
```

Flags required for implementation are kept private, flags needed by other libraries linking against it are set public.
I set my module build flags like this:

```
target_compile_definitions(mylib PRIVATE MY_FLAG)
```

I always use either `PUBLIC`, `PRIVATE` or `INTERFACE` when I express dependencies in CMake:

```
target_link_libraries(mylib
    PRIVATE
        foolib
        barlib
    PUBLIC
        json
    )
```

Here `mylib` is dependent on `foolib` and `barlib` for its implementation but anyone using `mylib` won't deal with anything related to `foolib` and `barlib` so these dependencies are private.
If `mylib` is returning a JSON object, for example, the JSON object definition is located in the `json` library and therefore should `json` be set as a PUBLIC dependency to appear on `mylib`'s public API.


* Public: interface dependencies
* Private: implementation dependencies

## Anti-Patterns

I always try to avoid these calls because they affect all targets:

* ⛔️ `INCLUDE_DIRECTORIES()`
* ⛔️ `ADD_DEFINITIONS()`
* ⛔️ `LINK_LIBRARIES()`

I also avoid using `TARGET_INCLUDE_DIRECTORIES()` with a path outside the library scope because that adds a hidden dependency on where is that library located relative to the callee.

## Specific Cases

If I have a header library I set it to be `INTERFACE`:

```
add_library(mylib INTERFACE)

target_include_directories(mylib INTERFACE include)

target_link_libraries(mylib INTERFACE bar)
```

## Example

In this [project](https://github.com/Labonneguigue/CarND-Path-Planning-Project) I implemented these concepts. There are still some bad practices I haven't removed which are due to the fork.

## Sources

This work is heavily based on [Mathieu Ropert's talk at CppCon: Using Modern CMake Patterns to Enforce a Good Modular Design](https://www.youtube.com/watch?v=eC9-iRN2b04) ([📄 slides](https://gist.github.com/mbinna/c61dbb39bca0e4fb7d1f73b0d66a4fd1)).

Here is an aggregator of the [best CMake content](https://github.com/onqtam/awesome-cmake) out there.