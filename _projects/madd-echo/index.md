---
layout: post
title: ECHO - Exploration of Celestial Homes for Observation (demo)
description: A prototype high-fidelity 3D test bed for simulating autonomous navigation capabilities of Mars planetary rovers in a controllable Mars-Analog environment. The test bed allows users to perform experiments which evaluate the outputs of autonomous navigation tasks (e.g., rover surface terrain image segmentation).


skills:
- C++
- Python
- Entity-Component Frameworks
- Unreal Engine's Graphical Blueprints
- 3D Modeling and Lighting
- Linux Shell Scripting
main-image: /echo_demo.png 
---

## Capabilities
- ROS 2 (foxy/humble) interfacing for processing and publishing Unreal Engine output to ROS 2 nodes and topics.
- Integration of You Only Look Once (YOLO) vision models via an external ROS 2 workspace.
- Control of lighting and hazardous weather conditions (e.g., Martian Sol day-night cycles and Mars sand storms).
- Taking rover surface imagery for synthetic datasets. 

{% include image-gallery.html images="echo_demo_1.png" height="400" %} "Discovery rover detects rock field at Site Marvin in control conditions" - the user-controllable rover, modeled after Mars Exploration Rovers (MERs) Spirit and Opportunity, runs image segmentation on a terrain class, rock field, at a designated site of interest in the simulator level landscape. This is in control conditions with midday lighting and no weather conditions.

{% include image-gallery.html images="echo_demo_2.png" height="400" %} "Discovery rover detects rock field at Site Marvin in Hazardous Sand Storm Conditions" - the user-controllable rover runs image segmentation while in a Mars sand storm. It can be observed that performance drops and the segmentation model no longer draws masks.
