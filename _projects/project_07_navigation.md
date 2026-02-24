---
title: "Perception Localization and Mapping for Mobile Robot"
excerpt: "<img align='left' src='/images/projects/ProjectNavigation.png' width='450' style='margin-right: 15px; margin-bottom: 15px;'/>**University Project + Extra Course -Completed** <br>
Robotics Perception Final Assignment - 2023 <br>
C++ - ROS1 - ROS2 - SLAM <br>
Implemented C++ ROS1 code to estimate the odometry of an autonomous shuttle from wheels encoders, based on real recorded data.
Mapped the laboratory using recorded LIDAR + odometry data, using gmapping.
Imported the map in a stage simulator and performed autonomous watpoint navigation.
Studied and tested from external udemy course the Navigation Stack for ROS2."
collection: portfolio
---

**Completed** - 2022 | C++ - ROS 1 - ROS2 - Nav2 - Odometry - SLAM 
<div class="project-github-link">
  <a href="https://github.com/AlePuglisi/perception-localization-mapping-projects" class="btn btn--inverse">GitHub Repo - University Project</a>
  <a href="https://github.com/AlePuglisi/navigation-learning/tree/main/nav2-course" class="btn btn--inverse">GitHub Repo - Course</a>
</div> 

## University Project 
Final group assignments of a course in [Perception Localization and Mapping for Mobile Robots](https://www11.ceda.polimi.it/schedaincarico/schedaincarico/controller/scheda_pubblica/SchedaPublic.do?&evn_default=evento&c_classe=837910&__pj0=0&__pj1=22e9c7f323b7d3a5839ccc4b7486a513).

Implementation of Mobile Robot navigation simulation with ROS1, using Real robot data collected in ROS bags.

- Implemented Odometry estimation for an autonomous shuttle, with ROS and C++.
- Mapped an indoor environment from ROS bag Laser Scan and 3D Lidar data, using slam_toolbox.
- Denoised the map, and performed autonomous navigation from csv waypoints, using AMCL (Adaptive Monte Carlo
Localization) for localization and Navigation stack for path generation and tracking.

### First poject
Main objectives: 
- Derived kinematic model of an autonomous shuttle.
- Used encoder wheel information to reconstruct the autonomous shuttle odometry.

### Second project
Main objectives: 
- Mapped the environment explored by a mobile robot, using data collected in a ROS bag.
- Used both 2D Lidar and 3D Lidar (converted in 2D information).
- Relied on a ros_stage simulation environment for Navigation.
- Tuned navigation parameters to optimize performance. 
- Performed autonomous waypoint-follow on that map, using points from a .csv file.

Read more details on the [repo README](https://github.com/AlePuglisi/perception-localization-mapping-projects/blob/main/README.md).

## ROS2 SLAM Course (Udemy) 

Course on Nav2 [by Edouard Renard](https://www.udemy.com/course/ros2-nav2-stack/?srsltid=AfmBOooiAWhc3jH4Gwttw345eHEBR6KJ7WLRfCRzbN5M8y_iSPS0GvtT&couponCode=KEEPLEARNING).

Exploring ROS2 open source libraries for Mapping and Navigation tasks, with a turtlebot robot in gazebo. 

Further details on each lesson on my [GitHub README](https://github.com/AlePuglisi/navigation-learning/blob/main/nav2-course/README.md) Notes.
