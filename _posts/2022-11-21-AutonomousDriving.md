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
Robotics Science and System (6.141) is MIT flagship robotics course. In this course, we learn about control, sensing, planning and localization and implement the algorithms in our robot on MIT racecar platform, which is based on Slash and very cool! Builiding an autonomous system like this is an exciting and challenging experience!

Videos!
===
[Final race](https://www.youtube.com/watch?v=MFKS91_Ywq0): Beneficial from our robust lane dectection algorithm and fine tuned pure pursuit controller, our lap time is less than 50s, the race car maintain a 4+m/s even when turnning!

[Partical filter and localization](https://youtu.be/r4zQ3zJ0SVs): Most rewarding part of the course! Seeing the localization algorithm we wrote actually works is awesome! I also implemented low variance resampling for the filter.

[RRT path planning and tracking](https://youtu.be/NvQlUep9JdY): Implemented sampling based method to search path given graph map.

[A* path planning and tracking](https://youtu.be/Gy9aFhdIT7A): Implemented heuristic search method to search path given graph map.

[Line follower and contrller test](https://youtu.be/OaXra8ETLHU): Building blocks for advanced tasks! We implemented pure pursuit controller and CV algorithm to detect and track certain path.


What I learned
===
Here are some thoughts I have after taking this amazing course. We also wrote down all our technical details and experiments charts, analysis in the [lab reports](https://rss2022-9.github.io/website/labs/). Check them out if interested!
1. Good teamwork is important for solving complicated engineering problem. As long as everyone in the team knows what they are doing and how they can push the team forward, the team can actually achieve a healthy balance and make progress. At the mean time, don't forget to communicate and praise team members!
2. Get your hand dirty. As an engineer, the best way to learn is combining theory and implementing together. I appreciate how much MIT values the hands-on experience. The course is very intense, even I have experience in ROS and autonomous roobt before, it's still challenging to build and make everything work in a short time. And this also pushes my understanding and skill to a new level.
3. Know more and see a bigger picture. Robot is a complicated system. To design a system to accomplish certain tasks, there are lots to consider. That's why konwing the characteritics of different techiniques are important, and analyzing the challenges we are facing and selecting the corret technical roadmap is even more important! Always good to see a big picture when you're working on something.
4. Technical sides:
   * A* vs RRT: it's interesting to see the comparison in real robot. Generally, RRT will find a suboptimal goal faster in large-scale map. But the scale of map is also determined by how we discretize the map. So comparing algorithms in real application and figure out when to use is important. For Stata map, A* is fast enough and provide an optimal solution.
   * Pure pursuit controller: it's very superprised to me how well this simple geometric controller can work on the vehicle. It's very smooth and tracking error is small in low speed case. But it also comes with some problems: the look-ahead distance is not easy to tune, and the controller can't handle high speed case esp. with aggressive path dynamics. I would like to combine it with other controllers like LQR in the future to account for vehicle dynamics and achieve better performance.
   * Particle filter: this sample-based Bayes filter shows how powerful it is when dealing with non-gaussian noise and localization problem. We also implemented low variance resampling to keep a variety of particles. One downside for PF is the computation. To simulate dyanmics for thousands of particles, compare, update is not a cheap process for on-board computer. Probably using GPU will accelerate this process.

Acknowlegements
====
This project was done with Nisarg Dharia, Nana Yeboah-Asare Jnr and Meenu Singh. We went through the nights spent in Stata basement together. Thanks for the support from Prof. Luca Carlone and wonderful TAs.

![car](/images/RSS/team.jpg "Our race car TBD")