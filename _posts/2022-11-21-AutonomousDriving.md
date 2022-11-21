---
title: 'Autonomous Driving Project'
date: 2022-11-21
permalink: /posts/2022/11/autonomous-driving/
tags:
  - robot
  - course project
  - autonomous driving
---

**We won 3rd place (aka podium!!) out of over 20 teams in MIT Robotics Science and System 2022 final challenge!**

![car](/images/RSS/MITracecar.jpg "Our race car TBD")

Introduction
===

Videos and what we did!
===
[Final race](https://www.youtube.com/watch?v=MFKS91_Ywq0): Beneficial from our robust lane dectection algorithm and fine tuned pure pursuit controller, our lap time is less than 50s, the race car maintain a 4+m/s even when turnning!

[Partical filter and localization](https://youtu.be/r4zQ3zJ0SVs): Most rewarding part of the course! Seeing the localization algorithm we wrote actually works is awesome! I also implemented low variance resampling for the filter.

[RRT path planning and tracking](https://youtu.be/NvQlUep9JdY): Implemented sampling based method to search path given graph map.

[A* path planning and tracking](https://youtu.be/Gy9aFhdIT7A): Implemented heuristic search method to search path given graph map.

[Line follower and contrller test](https://youtu.be/OaXra8ETLHU): Building blocks for advanced tasks! We implemented pure pursuit controller and CV algorithm to detect and track certain path.


What I learned
===


Acknowlegements
====
This project was done with Nisarg Dharia, Nana Yeboah-Asare Jnr and Meenu Singh. We went through the nights spent in Stata basement together. Thanks for the support from Prof. Luca Carlone and wonderful TAs. 