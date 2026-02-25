---
title: "Software Development, Simulation, Control, and Hardware Experiments on a Multi-Modal Quadruped Robot"
excerpt: "<img align='left' src='/images/projects/ProjectMultiModalRobot.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**Research Project at SRL - Completed** <br>
Research at the Space Robotics Lab - 2024 <br>
C++ - ROS2 - Gazebo <br>
Implemented and tested novel motion algorithms on a prototype multi-locomotion limbed robot. 
Updated the ROS2 joint control software for the new-end effector module. 
Updated the Gazebo simulation with the new robot components, and fine tuned its dynamic parameters.
Proposed a new stable locomotion-mode transition algorihtm. 
Fine tuned the servo motors controllers and tested the algorithms on the real system."
collection: portfolio
---
**Completed** - 2024 | C++  - ROS 2 - Gazebo Simulation - Limbed-robot - Hardware Testing 
<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/LIMBERO" class="btn btn--inverse">GitHub Repo</a>
  <a href="https://www.youtube.com/playlist?list=PLFgoOtxCJKTPv_dibdvSUT_YPGDJBc_5C" class="btn btn--inverse">YouTube Videos</a>
</div> <br>
<div style="display: flex; justify-content: center; align-items: center; gap: 5px;">
  <img style="width: 35%; max-width: 500px;" src="/images/projects/LIMBERO.png">
  <img style="width: 16%; max-width: 500px;" src="/images/projects/LIMBERO_GRIEEL.jpg">
  <video style="width: 45%; max-width: 500px;" autoplay loop muted playsinline>
    <source src="/images/projects/LIMBERO_GRIEEL.mp4" type="video/mp4">
  </video>
</div> <br>
This project was completed as a member of the Rover team, one of the many teams of the Space Robotics Lab, led by Yoshida Kazuya sensei.

The starting point was a ROS 2 software development of many packages controlling a climbing quadruped robot with 4 DOF per limb, and a gripper as an end-effector. 
What is the mind-blowing part? The new end-effector I worked with, both in simulation and in real life, was a transformable module, able to transition from gripper to wheel and vice versa, by pulling some wires. Making the robot able to walk, climb, and even drive!

**Summary**:
Conducted 500+ hours of research in Tohoku University’s largest robotics lab, which comprises 80+ members
across 5+ teams, under the supervision of Yoshida Kazuya Sensei.
- Researched methods for robustly and efficiently transforming a prototype multi‐modal limbed climbing robot,
equipped with a transformable Gripper‐Wheel module.
- Integrated the new module in high/low‐level control software, with a ROS2 architecture written in C++ and Python,
enabling efficient actuation of new joints in both modes.
- Improved Gazebo simulation reliability and ros2_control controller performance by fine‐tuning dynamical parame‐
ters and PID gains, obtaining a realistic simulation for algorithm testing, using Python to analyze performances.
- Tested the updated software and transition algorithm on the physical system, achieving system stability and elimi‐
nating steady‐state error in motor control.

**Objectives**:
- Update the ROS 2 software.
- Find a robust and stable way to transition between possible locomotions.
- Set up a reliable simulation in Gazebo.
- Tune the joint trajectory controllers, using ros2_control framework.
- Perform experiments on the real system.

**Main Contributions**:
- updated the ROS 2 code, now able to:
 - Manage the additional end-effector joints (3 more).
 - Start the transition procedure in a stable way, changing joints angle and pulling the wires.
 - Drive the wheels.
 - start a high-level algorithm that, using the classical legged robot stability criterion, transforms one 
 by one all end-effectors, keeping stability.
 - connect to the new Dynamixel motors, and set the internal PID gains to mine (overriding default 
 values), and control the motors.
- Fully Physically realistic simulation in Gazebo.
- Stable joint controller, with almost perfect tracking.
- Ability to maintain the limb raised, even with a so heavy end-effector. 
 Previously, the team had problems in transition because of incomplete PID tuning, my contribution 
 was very appreciated and improved significantly the performance. 
- Testing on the real hardware and achieving the desired stability.

**Exhange Research Presentation**
<iframe src="/files/projects/SRL_Presentation.pdf" width="100%" height="600" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>

<br>
**Research Summary**
<iframe src="/files/projects/SRL_Summary.pdf" width="100%" height="700" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>

<br>
**Research Report**
<iframe src="/files/projects/SRL_Report.pdf" width="100%" height="700" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>