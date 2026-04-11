---
layout: post
title: Pilgrim (TurtleBot3) Planetary Rover
description: Pilgrim is a ROS 2 TurtleBot lidar noise injection node in normal and dust / sandstorm conditions. I include a demo here for demonstration of TurtleBot3 navigation with ML-based LiDAR sensor noise injection and comparison.
skills: 
- ROS 2 Foxy
- Python
- Linux (Ubuntu 20.04)
- TurtleBot3
- Gazebo Classic
- RViz
main-image: /pilgrim_demo_1.png
---

## Research Inquiry:
Pilgrim is my application of Harvey Mudd College's CSCI-035: Computing Science for Insight with ROS 2, Gazebo, and TurtleBot to ask, "how does simulating weather condtions (i.e., Mars sand storms) influence the LiDAR measurements of a planetary rover (TurtleBot3's are standard for Lunar/Martian exploration research)?"

<div class="image-gallery-container">
  {% include image-gallery.html images="pilgrim_demo_1.png" height="400" %} "Pilgrim rover is traversing terrain with cubes, spheres, and a lambda" - this is the control scenario with no weather conditions.
</div>

<div class="image-gallery-container">
  {% include image-gallery.html images="pilgrim_demo_scan.png" height="400" %} "LiDAR measurements in RViz" - this is Pilgrim's LiDAR data of the terrain in  control conditions, visualized in RViz.
</div>

## Results:
<div class="image-gallery-container">
  {% include image-gallery.html images="lidar_noise_hist.png" height="400" %} A comparison of LiDAR data between control and sand storm conditions shows that LiDAR becomes less accurate in hazardous conditions. Be advised!
</div>
