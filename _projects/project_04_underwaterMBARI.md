---
title: "Simulation of MBARI's Underwater Vehicles"
excerpt: "<img align='left' src='/images/projects/ProjectMBARIsim.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**Personal Project - Ongonig** <br>
Underwater Simulation Project - 2026 <br>
C++ - Python - ROS2 - Gazebo - Stonefish <br>
Modeled ROV Doc Ricketts + robotic arm (sketchfab) in ROS2 + Gazebo(2025). 
Migrated Ricketts simulation to Stonefish simulator (2026).
Modeled the MOLA AUV (blender) consistent with MBARI's vehicle specification.
Integrated reconfigurable lights, proprioceptive (IMU, pressure) and exteroiceptive (DVL, camera, sonar) sensors.
Configured the simulation for ROS2 and implemented teleoperation. Modeled custom underwater worlds.
Tested perception and state estimation algorithms."
collection: portfolio
---

<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/MBARI-vehicles-sim-ros2" class="btn btn--inverse">GitHub Repo</a>
  <a href="https://youtu.be/2kjYHoX9uA8?si=bx9ndiEQMwIl3Mih" class="btn btn--inverse">YouTube Demo</a>
</div><br>
This personal project is inspired by the work of the [Monterey Bay Aquarium Research Institute (MBARI)](https://www.mbari.org/), which sparked my interest in marine robotics and continues to motivate my research journey.

As part of my PhD at the [RSM Team](https://www.lirmm.fr/equipes/rsm/) - LIRMM, I needed a realistic underwater simulation environment to prototype and test perception algorithms. I chose the Stonefish simulator for its lightweight architecture and physically realistic underwater rendering.
To explore its capabilities and integration within the ROS2 ecosystem, I began developing a simulation environment for two of my favorite MBARI [vehicles](https://www.mbari.org/our-work/technologies/vehicles/): the [MOLA AUV](https://www.mbari.org/technology/mola-auv/) (developed by the [CoMPAS Lab](https://www.mbari.org/team/compas-lab-control-modeling-and-perception-of-autonomous-systems-laboratory/)) and the [ROV Doc Ricketts](https://www.mbari.org/technology/rov-doc-ricketts/).

The project includes several development steps, from modeling the vehicles in Blender to configuring actuators and implementing teleoperation nodes in ROS2. More recently, I have started experimenting with high-level perception and mapping pipelines, including:
- Visual SLAM using ORB-SLAM3
- Fiducial AprilTag markers detection 
- 3D reconstruction using COLMAP and gsplat

The main accomplishments up to now are the following: 

- Migrated a previous personal underwater robotics simulation project from Gazebo to Stonefish.
- Defined physical‑visual realistic 3D models of MOLA AUV and ROV Doc Ricketts (modeled in blender). Integrated
thrusters actuation, teleoperation, and sensing, based on vehicle’s specifications and MBARI’s research papers.
- Tested state‑of‑the‑art computer vision and robotics algorithms on custom modeled world
(Kalman filtering, COLMAP SfM, gsplat, AprilTag, ORB‑SLAM3).

**Project Demo Video**
<iframe src="https://www.youtube.com/embed/2kjYHoX9uA8" 
  title="MBARI Simulation Demo"
  width="640" height="360"
  frameborder="0" 
  allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
  allowfullscreen>
</iframe>
<br>

**Project Overview Presentation**
<iframe src="/files/projects/MBARI_vehicles_sim_ros2.pdf" width="100%" height="600" frameborder="no" border="0" marginwidth="0" marginheight="0"></iframe>
<br>

Stay tuned, new simulation projects are under development! e.g. Lightweight manipulator for MOLA, acoustic SLAM with factor
graph (gtsam), deep sea animals tracking, autonomous navigation in coral reef restoration garden.
