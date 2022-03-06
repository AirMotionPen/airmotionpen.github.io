---
layout: post
title:  "Thought on IMU Approach"
date:   2022-02-02 11:00:00 -0500
categories: design
---

# Thought on IMU Approach

Thoughts on the IMU approach
1. The AHRS algorithm performs poorly on our MPU in terms of calculating Euler angles, there are heavy drifts and it’s much worse than the XIO’s demo. So if we want to accurately model the rotational motion, we could purchase the XIO NGIMU. But the NGIMU won’t help us model the translational motion with its linear acceleration measurement.

2. The IMU could provide accurate Euler angles to control cursor coordinate, but modeling the translational motion is impossible. At best, we can get linear acceleration without gravity, a translational motion consists of both accelerating and decelerating motions, so the motions will cancel out in terms of distance. So the best approach would be to use LED transmission like a normal mouse or only support in-air control, which will be accurate for daily usage.

3. In general, the NGIMU definitely provides really accurate measurements that the current IMU could not reach. It’s worth buying if we want accurate rotational measurements.

