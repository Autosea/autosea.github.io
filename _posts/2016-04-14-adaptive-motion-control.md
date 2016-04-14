---
layout: post
title: Adaptive Motion Control For Ships With Cascaded Nonlinear Feedback Control
---
## Background
Automated motion control of ships has been a research topic since the early 20th century. In recent years, the research has expanded from control of manned vessels to also include unmanned vessels. Challenges include handling uncertain nonlinear hydrodynamics and external disturbances, since the ocean is an unreliable environment with nonlinearities and unpredictable perturbations. Hence, it is important to develop adaptive and robust control algorithms, which can deal with these internal uncertainties and external disturbances in a realistic and energy efficient manner. It is also important to consider physical magnitude and rate saturation constraints for the actuators.

## Scope
The goal of this project work is to investigate a combination of adaptive and nonlinear feedback control algorithms to handle model uncertainties, external disturbances and actuator constraints.

## Proposed Tasks
1. Develop and implement cascaded nonlinear feedback control algorithms for a ship in Matlab/Simulink to address the problem of both magnitude and rate saturations for the actuators. 
2. Perform a literature study on state-of-the-art adaptive control algorithms.
3. Introduce uncertainties concerning the inertia matrix, control input vector and external disturbances for the ship model. Combine a selection of adaptive control algorithms from the literature study with the nonlinear feedback controllers, to handle both actuator constrains, uncertainties and disturbances.
4. Compare the closed-loop performance of the combined control algorithms using performance metrics.

The project work aims to be extended into a master thesis for the spring of 2017. While the project goal is to get an overview of existing solutions, and test and compare these solutions through simulations in Matlab/Simulink, the master thesis goal is then to further develop and implement new methods, and perhaps test and compare these through both simulations and using model-scale ships in the Marine Cybernetics laboratory, see (http://www.ntnu.no/imt/lab/cybernetics). Depending on the results, it can also be possible to perform full-scale experiments in the Trondheimsfjord associated with the Autosea project. The **master thesis tasks** include

1. Further develop the control algorithms from the project work such that they handle actuator constrains, uncertainties and disturbances in an energy efficient manner.
2. Implement and compare a newly proposed control algorithm with the previously tested algorithms in Matlab/Simulink.
3. If possible, test the performance of algorithms in the Marine Cybernetics labora- tory.
4. If possible, test the performance of algorithms in full-scale experiments.In this case, a ship model must be developed using system identification/multi-variate analysis based on collected data from full-scale sea trials.
5. Finally, combine the proposed "low-level" adaptive and nonlinear control algorithm with a "high-level" collision avoidance system, which will be provided by another MSc-student or the supervisors, to enable energy-efficient and precise collision avoidance capabilities.

## Supervisors 
Main supervisor: Morten Breivik (<morten.breivik@itk.ntnu.no>). <br />
Co-supervisors: Mikkel Sørensen (<mikkel.sorensen@itk.ntnu.no>) and Bjørn-Olav Eriksen (<bjorn-olav.holtung.eriksen@itk.ntnu.no>).