---
layout: post
title: Uncertainty management in scenario-based MPC for collision avoidance
category: COLAV
---
## Background
Collision avoidance (COLAV) methods typically attempt to deviate sufficiently from the desired path to ensure that no collision will occur. The decision about how much to deviate must be made in the presense of several different kinds of uncertainties. Even if other ships move along straight lines, imperfect sensors are needed to estimate their velocities, and these estimates may suffer from significant uncertainties. Such uncertainties are typically quantified using probability theory, e.g., by means of covariance matrices.

Most collision avoidance methods do not facilitate any probabilistic treatment of such uncertaintites. However, in the recently developed simulation-based model predictive control (SB-MPC) approach to collision avoidance, it is possible to include this kind of information in the cost function. 

![Different types of uncertainty]({{site.url}}/assets/uncertainties.png)

## Scope

A robust control strategy should incorporate possible control actions of other ships. Mitchell et al. 2005 (ref below) describe a method where safe reachable sets of an adversary game can be computed. This safe set is calculated based on the “worst” possible control by the adversary agent (quadrotor in this example: <a href="https://www.youtube.com/watch?v=HSFmGdI0TAY&start=1020">https://www.youtube.com/watch?v=HSFmGdI0TAY&start=1020</a>). For a COLAV application the focus should be on calculating the safe reachable sets under different conditions (COLREGS are followed, COLREGS are followed, but with uncertainty on when and which control is applied, COLREGS are not followed – but course and velocity is maintained etc.)

## Proposed Tasks for the 5th year project

1. Expand the work in "Uncertainty management in scenario-based MPC for collision avoidance" with kinematic data of target ship (e.g. include different classes of vessels and their associated maneuverability – capability of velocity and course changes).
2. Conduct a literature study on MPC and Reachable Sets for collision avoidance.
3. Implement a version of the Reachable sets for benign target vessels and compare with SB-MPC method.
4. Assess effect of uncertainty on Reachable sets method compared to its effect on the SB-MPC.
5. Write report. 

## Proposed Tasks for the master thesis

The project work aims to be extended into a master thesis for the spring of 2018.  Possible projects include the following:

Project A: Bayesian control methods through Machine learning (Gaussian processes)
1. Literature review of probabilistic control methods (see e.g. Jain, A. et al 2018 and Kocija, J. 2016 “Modelling and Control of Dynamic Systems Using Gaussian Process Models”)
2. Implement a probabilistic control based on the SB-MPC used in the 2017 project
3. Assess effect of probabilistic control

Project B: Target vessel uncertainty
1. Define relevant “uncertain” scenarios for the different classes of target ships (e.g. Base case is that all vessels adhere to COLREGS, however; A sailboat may not have power to maneuver; A daycruiser might not adhere strictly to COLREGS; A kayak may not be able to maneuver fast enough; A supertanker’s maneuverability in a strait may be limited by draft depth; etc.)
2. Assess the effect of uncertain behavior of target vessels will affect the available maneuverability space of the SB-MPC
3. Incorporate the added uncertainty from the uncertain scenarios in the SB-MPC method used in the 2017 project, and assess the associated risk with each scenario (i.e. combining the effect of the assessed scenario with its associated uncertainty – e.g. a daycruiser is much more likely to not adhere to the COLREGS than a commercial vessel, etc.)

Project C: Detection uncertainty of target vessels
1. Define scenarios which will affect the uncertainty of the kinematic data of the detected target vessels (i.e. fog, rain, heavy seas, obstacles, missing sensors, erroneous sensor readings, etc.)
2. Assess how the added uncertainty in target vessel kinematics affect the available maneuverability space of the SB-MPC
3. Incorporate the added uncertainty from the uncertain kinematics in the SB-MPC method used in the 2017 project, and assess the associated risk with each scenario (i.e. combining the effect of the assessed uncertainty in the kinematics)

## Autosea
The candidate will be associated with the AUTOSEA project, which is a collaborative research project between NTNU, DNV GL, Kongsberg Maritime and Maritime Robotics, focused on achieving world-leading competence and knowledge in the design and verification of methods and systems for sensor fusion and COLAV for ASVs. The project has access to supervision and physical test platforms through our industry partners.

## Contact
* Main supervisor [Edmund F. Brekke](http://www.ntnu.no/ansatte/edmundfo)
* Co-supervisor [Simen Eldevik](Simen.Eldevik@dnvgl.com)
This project is proposed by DNV GL.

## References

* I.M. Mitchell, A.M. Bayen and C.J. Tomlin (2014): “[A time-dependent Hamilton-Jacobi formulation of reachable sets for continuous dynamic games](https://ieeexplore.ieee.org/document/1463302/)”, IEEE Transactions on Automatic Control.
