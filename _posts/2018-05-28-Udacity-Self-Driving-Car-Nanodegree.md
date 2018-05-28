---
toc: true
header:
    image: ./images/udacity.png
---

_I have now completed the nanodegree from Udacity. It was an incredible learning experience. I'll first go through the pros and cons of this program and then I'll list all the projects I had the opportunity to work on._


### 👍 Pros

First, I highly appreciated the lessons, I found them thorough and well thought. The instructors made it very easy for me to understand every concept, for example, I couldn't fully understand Kalman Filters out of University but after Sebastian Thrun's lesson I could apply them in several Nanodegree projects but more importantly I could use one at work.

On top of the content covered in the lessons, they give some links to more in-depth materials for students to dig even deeper into a particular topic. For each project, plenty of resources are provided (such as purpose-built simulators) which encourage the students to spend more time than is required to make their implementation stand out.

A great community. The Slack workspace is always very active and you won't wait long to have your question answered.

### 👎 Cons

I believe that there should be more focus on algorithms efficiency, runtime and code quality.
The code reviews were too permissive in my opinion.

### ⭐️ Conclusion

Overall, I would recommend the Self-Driving Car Nanodegree to anyone interested in this field!

---

Here is my collection of repositories containing my solution to each SDCND projects.

## 📚 Term 1 - Computer Vision & Deep Learning

### ✏️ Project 1 - Lane Lines Detection

This project was very informative since it covered very important topics of the *classical* Computer Vision space such as Hough Transforms and Canny Edge detection. The objective was to detect lane lines.

[Here is more about it.](https://labonneguigue.github.io/CarND-LaneLines-P1/)

### ✏️ Project 2 - Traffic Sign Classifier

The second project was my first attempt at using Deep Learning. I build a Convolutional Neural Network for traffic sign classification. 

[Project is that way.](https://labonneguigue.github.io/CarND-Traffic-Sign-Classifier-Project/)

### ✏️ Project 3 - Behavior Cloning

The goal of this project was to enable a car to drive by itself in a simulator. After collecting some data where I was manually driving it, Through the use of Transfer Learning, I trained the last layers of a neural network to perform a regression task on the steering angle.
I only needed to record 2 lapses thanks to my ability to augment the collected dataset.

[Project write-up right here.](https://labonneguigue.github.io/CarND-Behavioral-Cloning-P3/)

### ✏️ Project 4 - Advanced Lane Finding

This project is very similar with the first one, the only different is that the approach is more robust and can accommodate for lane curvature. I changed the perspective before trying to detect the lane markings.

[Description of my project solution.](https://labonneguigue.github.io/CarND-Advanced-Lane-Lines/)

### ✏️ Project 5 - Vehicle Detection & Tracking

For a self-driving car to operate safely, it needs to know if there are some cars around and where. In this project I trained a Support Vector Machine (SVM) to classify whether a image patch contained a car or not using an Histogram of Oriented Gradients (HOG) descriptor. 

[Project details.](https://labonneguigue.github.io/CarND-Vehicle-Detection/)

## 📚 Term 2 - Sensor Fusion, Control and Localization

The second term of this NanoDegree was focused on **Sensor Fusion**, **Control** and **Localization**. I believe that these are the domains that are crucial today to develop ADAS systems that are going to increase driving safety significantly.

### ✏️ Project 6 - Extended Kalman Filter (EKF)

The Kalman Filters course was a great reminder from University. After the Extended Kalman Filter lesson, I applied one to the Sensor Fusion problem that face AVs. To navigate an uncertain and always evolving environment, AVs must receive data from different sensors types which are complementary to each other. The sensors provide data in different formats and each have their advantages and drawbacks.

[Have a look at that project writeup.](https://labonneguigue.github.io/CarND-Extended-Kalman-Filter-Project/)

### ✏️ Project 7 - Unscented Kalman Filter (UKF)

For this project I was provided with a simulator and some noisy data from 2 different sensors, a LIDAR and a RADAR, of a moving car. My task was to remove the noise from the sensor data using an UKF and give a best estimate of where the car is.

[More about my implementation of the UKF here.](https://labonneguigue.github.io/CarND-Unscented-Kalman-Filter-Project/)

### ✏️ Project 8 - Kidnapped Vehicle

Given a very similar environment as the previous project, my new task was to predict where the car was given only the distances to observable landmarks. [I used a particle filter to solve this problem.](https://labonneguigue.github.io/CarND-Kidnapped-Vehicle-Project/)

### ✏️ Project 9 - PID Controller

This very short project is a good reminder for every Software Engineer out there about System Control. A Proportional Integral Derivative Controller is very simple but also very effective. I managed to make my simulator car drive by itself only by knowing its cross-track error. [Check it out.](https://labonneguigue.github.io/CarND-PID-Control-Project/)

### ✏️ Project 10 - Model Predictive Control


[Project.](https://labonneguigue.github.io/CarND-MPC-Project/)

## 📚 Term 3 - Path Planning, Systems & Integration

### ✏️ Project 11 - Path Planning

For this project Udacity provided us with a simulator where I can control a car on a highway, the goal being to plan a smooth and accident free path with regard to the other cars on the road. The simulator provides data about the surrounding cars as well as data about the map. I build my path planner by assembling together the following 3 essential modules of a Self-Driving Car:

* Behavior Planner
* Trajectory Generator
* Predictor

[Check out how I managed to successfully complete this project here.](https://labonneguigue.github.io/CarND-Path-Planning-Project/)

### ✏️ Project 12 - Functional Safety

I was happily surprised to see this topic as part of a project. It is, in my opinion, a major topic in the Autonomous Driving space which does not get all the coverage it should have.

[Here is what I've learned and the documents I've redacted for a case study.](https://labonneguigue.github.io/CarND-Functional-Safety-Project/) 

### ✏️ Project 13 - Semantic Segmentation

It is definitely important for a self-driving car to know where is the road. In this project, I trained a Fully Convolutional Neural Network (FCN) to classify each pixels in the image to be labeled `road` or `not road`. [Here is the project](https://labonneguigue.github.io/CarND-Semantic-Segmentation/).

### ✏️ Project 14 - System Integration

Writeup not ready. 🛠



---