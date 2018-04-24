---
layout: post
title: Camera Positioning for Unmanned Ships
category: SF
---

| <img src="{{site.url}}/assets/revolt2.png" width="570"> |

## Background

The ReVolt is an unmanned and zero-emission ship concept designed for short sea shipping along the coast of Norway. The ReVolt was design for low energy demand and the propulsion system is fully electric. The ReVolt has 2 stern pods and 1 retractable azimuth thruster in the bow.

A 1:20 scale model of the ReVolt has been built to explore and demonstrate the vessels autonomous capabilities and to test other design features.

Today, the scale model of the ReVolt vessel only includes sensors for estimating own position and motion, but is missing sensors for observing the world around. The ReVolt model do have the possibility to log data, but is missing a communication system for transmitting the logged data onshore and receiving data from onshore. 

Two students are working on the ReVolt model this year and they have equipped the model with necessary sensors to achieve DP capabilities. During their project last fall, the students developed simplified DP controller and performed experiments in Trondheim Havn using the the ReVolt model. The students are now improving the DP controllers and they will also include the DNV GL thruster allocation algorithm into their DP controller.

Some media attention:
* [http://trondheimhavn.no/nyhet/norsk-skipsteknologi-pa-tysk-tv-1248.aspx](http://trondheimhavn.no/nyhet/norsk-skipsteknologi-pa-tysk-tv-1248.aspx)
* [https://www.youtube.com/watch?v=AyFkOfD1II8](https://www.youtube.com/watch?v=AyFkOfD1II8)
* [http://trondheimhavn.no/nyhet/tester-trondheims-forste-forerlose-ferge-1221.aspx](http://trondheimhavn.no/nyhet/tester-trondheims-forste-forerlose-ferge-1221.aspx)

Focus areas:
* IoT device: Make the physical ReVolt model an IoT device which can log and transmit live data to onshore data center and at the same time control the ReVolt model from this data center. Online comparison and validation against the digital twin should also be possible. 
* Control strategies: Using the physical ReVolt model with the new sensor package, implement different control strategies (including collision avoidance) and perform several model experiments to test and validate the implemented algorithms. 
* Virtual world  modelling: To be able to perform simulator based testing of the collision avoidance algorithms, some kind of virtual world modelling needs to be done e.g. simulation of marine traffic and sea/terrain.
* Sensor implementation: Implement models of the new sensor package on the Digital twin. Several sensors will "see" the same surroundings, how to ensure that all sensors have the same map of the world? The simulator will be used for both functional and failure testing of several systems needed for doing autonomous navigations. What is realistic sensor errors and how should this be implemented? Perform several simulations verifying the simulator capabilities.
* Design and verification of safety critical systems : Analyse the ReVolt model and system by using the STAMP analysis method to establish safe design requirements and verification objectives.  The analysis can be done several times as the ReVolt model system is developed and equipped further towards more autonomy.  Present safety standards and how they can be combined with STAMP is also interesting.

Main supervisor: [Morten Breivik](http://www.ntnu.no/ansatte/morten.breivik). <br />
Co-supervisors: Edmund Brekke, Tom Arne Pedersen (DNV GL), Øystein Engelhardtsen (DNV GL). For "Design and verification of safety critical systems": Mary Ann Lundteigen and Jon Arne Glomsrud (DNVL GL).
