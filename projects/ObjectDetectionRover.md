---
layout: project
type: project
image: img/rover.png
title: "Object Detection Rover"
date: 2025-11-01
published: true
labels:
  - Python
  - Raspberry Pi
summary: "This autonomous mecanum rover bridges embedded kinematics with high-level computer vision to create an accessible robotics education platform."
---

<div class="text-center p-4">
  <img width="200px" src="../img/micromouse/micromouse-robot.png" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-robot-2.jpg" class="img-thumbnail" >
  <img width="200px" src="../img/micromouse/micromouse-circuit.png" class="img-thumbnail" >
</div>

While a microcontroller handles low-level motor functions, the rover's autonomy is driven by a Raspberry Pi, where I engineered the core target detection software. The vision program runs in a dedicated thread parallel to the rover's search logic, continuously analyzing live PiCam frames.

Using color-segmentation, the system isolates purple targets and extracts centroid and radius data to guarantee high detection confidence. Once a target is verified, this event instantly overrides the sweep behavior and issues a real-time, full-stop command to the underlying hardware.
