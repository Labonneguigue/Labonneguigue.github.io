[adas-adoption]: ../images/adas_adoption.png "adas-adoption"
[isa]: ../images/isa.tiff "isa"

_Abstract: I'm looking at safety in the automotive sector and giving my thoughts on how it could be improved._

## The Accepted Road Toll 

1.25 million people are killed on the road each year in the world. With over 100 people dying in a motor vehicle crash per day in the US alone, it is the equivalent of a Boeing 777 falling from the sky every 3 days. This analogy is incredibly striking. The media coverage is nearly nonexistent.

The acceptance we have towards road death remains inexplicable to me.

The solution❓

**ADAS (Advanced Driver Assistance Systems).**

An ADAS is a system embedded in a vehicle which provides functionalities to increase overall road safety. Crash avoidance, crash severity mitigation and protection and post-crash phases are the main purposes of ADAS.

## The Slow Adoption of ADAS

Advanced Driver Assistance Systems (ADAS) are most definitely increasing the safety in our cars but their adoption is rather slow. Let's first look into why. This [McKinsey study](https://www.mckinsey.com/industries/semiconductors/our-insights/advanced-driver-assistance-systems-challenges-and-opportunities-ahead) provides some insights.


![alt text][adas-adoption]

The first observation is that generally people have low awareness that these system even exist. Advertisement seems insufficient. 

This fact might also be due to the naming confusion. This [website](http://howsafeisyourcar.com.au/) lists the different names the same system can have for different car manufacturer. Let's take an example:
The [Autonomous Emergency Braking (AEB)](http://howsafeisyourcar.com.au/aeb/) functionality warns the driver about an abrupt deceleration of the car ahead which might result in a collision and ultimately takes action autonomously to apply the brakes if the driver does not respond at all or quick enough. Here are a few example of how some car manufacturers have branded this system:
* Audi: *Pre Sense Plus*
* BMW: *Driving Assistant Plus*
* Ford: *Active City Stop*
* Honda: *Collision Mitigation Braking System*
* Mercedes-Benz: *PRE-SAFE Brake*
* Volkswagen: *City Emergency Braking*
* Nissan: *Intelligent Emergency Braking with Forward-Collision Warning*

(Nissan's designation is not easy to remember but give a better sense of what it does...)

I understand very well that each of these systems have a different implementation by the OEM or their Tier1/2 supplier which result in different sensitivity and user experience but they should all generally behave in a same way.

Far from me the wish to commoditize each ADAS where I think lies a great differentiating factor for companies but there should be some form of standardization in the naming convention.

For the average customer whose only knowledge about cars is knowing where the gas pedal is, knowing what is "Driving Assistant Plus" or "PRE-SAFE Brake" is supposed to perform might be a tough one. In the end the choice might be none and a degraded overall safety of the purchased vehicle. A shame since the vast majority of people are convinced once they've tried an ADAS once: almost 90% in the US.

Some proper education needs to happen.

## Mandating ADAS

The responsibility to spread ADAS across the auto market does not entirely fall onto the OEMs. In the EU, the European Commission (EC) has the ability to mandate the fitting of any particular ADAS on motorised vehicles.

As far as I'm aware, the only 2 mandatory fitting of ADAS in the EU are the following:
* Electronic Stability Control (ESC) Systems on all vehicles (from 1 Nov 2011 for new types of vehicle and 1 Nov 2014 for all new vehicles)
* Autonomous Emergency Braking (AEB) and Lane Departure Warning (LDW) Systems on heavy-duty vehicles (from 1 Nov 2013 for new types of vehicle and 1 Nov 2015 for all new vehicles) 

I believe that the approach is too slow and that we should widespread faster. We have so much technology already available to reduce significantly the number of deaths on the road. Here is a non-exhaustive list of safety systems which I believe **should already be mandatory on all new models.**
Throughout the rest of the article I'll ofter be referring to [this great report from the European Road Safety Observatory (ERSO)](https://ec.europa.eu/transport/road_safety/sites/roadsafety/files/ersosynthesis2016-adas15_en.pdf) released in 2016.

### Lane Departure Warning (LDW)

This camera-based system warns the driver when a lane line is unintentionally crossed or about to be crossed. The feedback can be of multiple forms:
* Haptic feedback: a small amplitude high frequency oscillation is applied on the steering wheel.
* Visual feedback: Blinking lights on the dashboard or in the Head-Up Display (HUD).
* Audible feedback.

Whenever the onboard camera responsible for that function detects that the car is about to cross a line without having the correct direction indicator enabled, the warning is triggered.

Without having the possibility to disable the system and the correct choice of (annoying) feedback from the car manufacturer, eventually, the driver should prefer to use the direction indicator instead of being lectured by the car over and over again.

Every driver experience skill atrophy along the years. I believe that such a system could **continuously teach** the driver or at lest maintain his/her current level of skills.

### Driver Monitoring System (DMS)

With the rise of better infotainment systems and wider screens in our latest cars as well as our constant need to check upon our smartphones, drivers have more and longer inattentiveness periods behind the steering wheel. Each time we take our eyes off the road, we might run over a cyclist, a pedestrian, crash into another car… This behavior is not acceptable and the car should prevent us from doing so. A Driver Monitoring System can detect in which direction the driver is looking and can correlate that with the current speed of the car and the upcoming road trajectory to determine if the driver is focused or not. Drowsiness can also be detected by such a system and a request to stop the car and take a break could be emitted. Finally, most advanced system can evaluate the cognitive load/distraction of the driver. 
This [page](https://www.vti.se/en/news/vehicle-driver-monitoring-sleepiness-and-cognitive-load/) provides more information regarding how such a system works.

In this [article](https://www.denverpost.com/2017/10/17/distracted-driving-smartphones/) Jennifer Smith says “We all know what’s going on, but we don’t have a breathalyzer for a phone.”.

Actually, **we do**.

Have a look at the Car Glance Classification system Lex Fridman built at MIT as part of his class entitled *Deep Learning for Self-Driving Cars*. 

<iframe width="560" height="315" src="https://www.youtube.com/embed/ShxbqjnsB8c" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<br/>

*Note: This is a custom-made retro-fitted system. It does not exist in commercially available Tesla models.*

The system described in the video detects where the driver is looking. From the date of the video, this quite mature system was already available in August 2016. It seems obvious to me that in the case where the driver is lacking attention such a system coupled with a disincentivizing haptic feedback in the steering wheel, audible warnings as well as visual cues would rapidly bring back his/her focus on the road ahead. 

The most compelling argument for incorporating this type of system in our cars is that, again, it continuously teaches the driver how to drive in a safely manner.

Finally, after watching this film *From One Second To The Next* from Werner Herzog, don’t you think that these fatalities could not have been avoided using a Driver Monitoring System ?

<iframe width="560" height="315" src="https://www.youtube.com/embed/_BqFkRwdFZ0" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

The National Highway Traffic Safety Administration (NHTSA) estimated that over 10% of road fatalities in the US in 2016 are associated with distracted drivers.

### Intelligent Speed Assistance (ISA)

From ERSO's report:

> ISA is a system which informs, warns and discourages the driver to exceed the statutory local speed limit or other desired speed thresholds below this limit at safety critical points.

Here is a video to explain how Ford chose to implement it on the S-MAX:

<iframe width="560" height="315" src="https://www.youtube.com/embed/F3qmtEGGlOo" frameborder="0" allow="autoplay; encrypted-media" allowfullscreen></iframe>

<br/>

**<center>Studies have shown that around 30% of fatal crashes are due to speeding.</center>**

The effectiveness of ISA has demonstrated by several studies such as the one conducted by [PROSPER](https://trimis.ec.europa.eu/project/project-research-speed-adaptation-policies-european-roads#tab-results).

![alt text][isa]

These results show that ISA could reduce fatalities by half.

The financial incentive is also very strong since the benefit to cost ratio of mandating ISA on all new cars is around 4. All add up to make a very compelling case for ISA.

Finally, the real difficulty in deploying ISA is the human-machine interface. The system needs to find the right balance between too much intervention which might result in a general disapproval from the public and a major set back for the OEM and his brand and too little intervention which would have no effect on safety. 

Include data from https://www.youtube.com/watch?v=SoZLrZTnUGs 

### Alcohol Interlock System

I kept this one for the end because the technology is not there yet but is very promising.

**<center>« Every year in the U.S., drunk driving claims approximately 
10,000 lives and costs approximately $194 billion. »</center>**

Such as speeding, drunk driving is responsible for about another third of road fatalities.

Nobody should have the right to drive drunk because in most cases, the victim is not the drunk driver. The victim is a pedestrian, a cyclist or another driver. 

To prevent driving under the influence, the [Driver Alcohol Detection System for Safety (DADSS)](https://www.dadss.org) is working on non-obtrusive methods. The one I prefer is the touch-based system where the alcohol level would be measure using an infrared light sensor when the driver touches the start button.

This method would remove the need to blow into the interlock device and wait about a minute to have permission to turn on the car. I goes without saying that method (only used as after-market device for recidivist drunk drivers) is a no-go. 
 
## The Self-Driving Cars of Tomorrow ? 

Am I loosing my time trying to fit ADAS into our cars when we'll have self-driving car tomorrow ?

I am not. Self-Driving Cars are the future and they will arrive ... **in the the future.**

The roads will be shared between human-driven vehicle and autonomous vehicle for another 50 years minimum.

Previsions forecast 1 billion vehicles on the roads by 2030 and most of them will be human-driven and built in the next couple of years. In the future, Self-Driving Cars will provide significantly increased safety in their segment of the market but if we want safer roads overall we need to act now and start mandating well designed ADAS solutions on all our human-driven cars.

---

Sources: 

* 📄 [European Road Safety Observatory (ERSO) 2016 Report](https://ec.europa.eu/transport/road_safety/sites/roadsafety/files/ersosynthesis2016-adas15_en.pdf)

* 📄 [European Commission > Vehicle Safety Systems](https://ec.europa.eu/transport/themes/its/road/application_areas/vehicle_safety_systems_en)