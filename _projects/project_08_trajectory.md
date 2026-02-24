---
title: "Trajectory Tracking Control of a Car-Like Robot"
excerpt: "<img align='left' src='/images/projects/ProjectTrajectory.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**University Project-Completed** <br>
Control of Mobile Robot Final Assignment - 2023 <br>
C++ - ROS1 - Simulation  <br>
Simulated a car-like (ackerman) robot with the simplified bicycle model, using ROS1 and a custom C++ numerical simulation (with odeint).
Analyzed the simulation with a simple kinematic or a complete dynamic model, designed and tuned a 
feedback linearization with PI jectory tracking controller.
Implemented the trajectory generator and the controller in C++."
collection: portfolio
---

**Completed** - 2023 | Simulation - ROS 1 - Mobile Robot Trajectory Tracking - C++ 
<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/bicycle-feedback-linearization-ros" class="btn btn--inverse">GitHub Repo</a>
</div> <br>

Final assignment of a course on [Control of Mobile Robots](https://www11.ceda.polimi.it/schedaincarico/schedaincarico/controller/scheda_pubblica/SchedaPublic.do?&evn_default=evento&c_classe=837146&lang=IT&__pj0=0&__pj1=8379d6c35eccfe1c998db9b2de7c0e1c). 

- Simulated a car‐like robot with kinematic and dynamic bicycle model, using ROS and odeint C++ library.
- Designed and Implemented a PI trajectory tracking controller with feedback linearization, with C++,
relying on Bode theory for controller tuning.
- Analyzed controller performance for different kinematic/dynamic models, using Python to read and plot ros bags.
- Maintained tracking error below 3% in x and y coordinates, over a trajectory with a 2‐meter amplitude.

Using the bicycle model, a car-like robot was simulated using ROS1 and a differential equation solver. 
Instead of using some classical tools like Gazebo or other physical simulators, the dynamic model (in the form of ordinary differential equations, from state space) has been implemented in 𝐂++ and simulated with the 'odeint' library. Both the Kinematic and Dynamic models have been analyzed and controlled. 

**Objective**:
- Develop a ROS 1 workspace with multiple packages to simulate and control the robot.
- implement a feedback linearization controller and PI trajectory tracking, as ROS 1 node.
- Follow a 2-meter amplitude 8-shaped trajectory in the x-y plane, with a period of 2 seconds. 
- Achieve the best possible tracking performance, by tuning the controller, both with the kinematic 
 and the dynamic model. 
- For dynamic model simulation, use 𝐝𝐢𝐟𝐟𝐞𝐫𝐞𝐧𝐭 𝐭𝐲𝐫𝐞 𝐦𝐨𝐝𝐞𝐥𝐬. 

**Reults**:
- Initialized a structured ROS1 workspace
- model-based and iterative tuning procedure: 
  - perfect tracking with Kinematic model simulation, with wrrors in the x and y
 directions always below 0.06 meters.
  - Simulated with linear tyre model, achieving trajectory racking 𝐞𝐫𝐫𝐨𝐫 𝐛𝐞𝐥𝐨𝐰 0.1 𝐦.
  - Discovered the limitations of the feedback linearization, based on the kinematic model, it was 
 impossible to achieve satisfactory performance for a more complex tyre model.

<iframe src="/files/projects/Trajectory_Tracking_Report.pdf" width="100%" height="700" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>