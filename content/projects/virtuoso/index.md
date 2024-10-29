---
title: Adaptive object detection algorithms for resource constrained autonomous robotic systems
date: 2023-08-01
tags:
  - GPU Resource Contention
  - Edge Computing
  - Perception
  - Computer Vision
  - Autonomous Driving
  - Object Detection

image:
  caption: 'Demonstration of an object detector with contention using high latency and low latency parameters. With contention and higher latency parameters, the detector will skip while running inference. The low latency parameters can keep latency low while maintaining an acceptable level of accuracy.'
  preview_only: false

featured: true

---

In this project, I worked with the Army Research Lab to implement a contention aware framework to be used with their autonomous unmanned ground vehicles. A contention aware framework means that a controller is aware of the resources that are available on the GPU. If all resources are available on the GPU, then the controller will scale all parameters of the perception model up to maximize accuracy. If the GPU is under high load because of other models required for autonomous driving, then the controller will scale down the parameters of a perception model to reduce latency at the minimal cost of accuracy. 

<!--more-->