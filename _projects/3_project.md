---
layout: page
title: Object Tracking
description: Object Tracking Using Kalman Filters for Single and Multiple Targets
img: assets/img/kalman1.png
importance: 3
category: work

---

The project focuses on the development of an algorithm that utilizes Kalman filters for tracking multiple objects in real-time settings. This is particularly essential in various practical scenarios such as airport security checkpoints, traffic signal monitoring, and surveillance systems where the simultaneous tracking of multiple objects is imperative. By employing a fixed camera to capture the scene and extract relevant data, the algorithm aims to efficiently track moving objects as they traverse the monitored area.

Through the utilization of Kalman filters, the algorithm predicts the future coordinates of each object by creating a bounding box around them. This predictive capability is instrumental in accurately tracking the trajectory of multiple objects simultaneously. The effectiveness of the algorithm is put to the test through evaluation on two distinct datasets - one containing a single car for tracking and another featuring multiple dice. The project's outcomes demonstrate the algorithm's robustness in tracking multiple objects under dynamic and real-time conditions. The implementation of Kalman filters for object tracking not only enhances the overall surveillance and monitoring processes but also showcases the algorithm's adaptability and effectiveness in scenarios where the tracking of multiple objects is essential for operational success.

{% include figure.html path="assets/img/kalman2.png" title="Governing formulae for object detetction using kalman filters" class="img-fluid rounded z-depth-1" %}

The implications of this project include, but are not limited to, improving the shopping experience at self-checkouts in retail stores, making self-checkout terminals more efficient and user-friendly.
