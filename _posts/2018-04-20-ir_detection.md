---
layout: post
title: Detection of ships in infrared data
category: SF
---
## Background
The Autosea project in colloboration with [AMOS](http://ntnu.edu/amos) aims to build knowledge that enables autonomous collision avoidance for maritime surface vehicles. In addition to ship instrumentation such as RADAR and AIS, a human navigator relies on his vision as an important tool to avoid collisions at sea. The International Regulations for Avoiding Collisions at Sea (COLREGS) explicitly states that navigators should use their vision in addition to RADAR. However, since cameras suffer from serious limitations without daylight, night cameras using infrared (IR) radiation are also needed on autonomous ships.

## Scope
Obstacle avoidance is a requirement for autonomous ship operations. Therefore, other objects in the planned path of the ship need to be identified and tracked. Object detection with an IR camera is one way to detect objects. However, this is challenging in maritime environments since objects at sea can be hard to distinguish from the waterline or hidden in waves. Furthermore, cameras have a limited range and objects far from the camera might be impossible to detect or cluttered by noise or other objects. In this project detection of marine vessels are the main priority. The algorithms developed in this project are not required to run in real-time, the focus is on detection performance and evaluation.

![Infrared image taken from an UAV]({{site.url}}/assets/infrared.jpg)

This project will look into object detection in IR images with two different approaches. The first approach is to investigate if objects at sea can be detected by a IR camera placed onboard the ship. The second will look into the use of an unmanned aerial vehicle (UAV) as an airborne sensor to detect objects. Both of these approaches have advantages and one important part of the project is to compare these.

## Proposed Tasks for the Specialization Project

1. Perform a litterature review over camera detection theory and usage of infrared cameras in a maritime context.
2. Evaluate detection algorithms and propose a suitable solution for maritime object detection.
3. Implement a detection algorithm using e.g. OpenCV/Matlab/Python.
4. Evaluate performance metrics of the detection algorithm.
5. Present the results and discuss limitations and challenges.

## Proposed Tasks for the Master Thesis

The MSc thesis may focus on a combination of different tasks, depending on the interests of the student.

- Conduct data acquisition experiments using IR equipment on Telemetron or the autonomous ferry prototype.
- Extend the detection method to a method for target tracking using IR data.
- Propose and test methods for fusion between IR and other sensors, such as optical cameras, lidar or radar.
- Refine the detection method from the specialization project, and/or investigate alternative detection methods.

## Prerequisites
This is a list of *recommended* prerequisites for this master project.

- Experience in either Matlab, Python or C++.
- Basic knowledge of computer vision or image processing. [TDT4265](http://www.ntnu.edu/studies/courses/TDT4265) is great, but not required.
- TTK25 Computer Vision for Control should be taken together with this project.

## Autosea
The candidate will be associated with the AUTOSEA project, which is a collaborative research project between NTNU, DNV GL, Kongsberg Maritime and Maritime Robotics, focused on achieving world-leading competence and knowledge in the design and verification of methods and systems for sensor fusion and COLAV for ASVs. The project has access to supervision and physical test platforms through our industry partners.

## Contact
Main supervisor [Edmund F. Brekke](http://www.ntnu.no/ansatte/edmundfo)<br />
Co-supervisor [Håkon Hagen Helgesen](https://www.ntnu.no/ansatte/hakon.helgesen)
