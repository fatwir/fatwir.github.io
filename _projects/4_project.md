---
layout: page
title: Photo Realistic Synthetic Image Generation
description: A project aimed at creating synthetic images to train object detection models
img: assets/img/project_2.jpg
importance: 2
category: academic

---

This project focusses on the generation of photo-realistic synthetic images in both 2D and 3D formats with the aim of better training object detection models. 

One of the major achievements of this project was the acceleration of the training process by almost 20%. This was achieved by employing Fully-Fused MLPs to train and validate a custom object dataset comprising around 170 images. 

Additionally, the project also achieved a validation PSNR of 25.96 dB when training a Neural Radiance Field. The achievement demonstrated a marginal 0.6 dB deviation from the original implementation and, crucially, managed to reduce the training time by almost half. These achievements came about as the result of the project's focus on reducing computational cost and improving training efficiency. 

To note, the entire study was applied to solve problems associated with retail self-checkouts, and the results were promising in terms of increased accuracy and speed of object detection. 

{% include figure.html path="assets/img/2.jpg" title="Pipeline used to generate images" class="img-fluid rounded z-depth-1" %}

The implications of this project include, but are not limited to, improving the shopping experience at self-checkouts in retail stores, making self-checkout terminals more efficient and user-friendly.
