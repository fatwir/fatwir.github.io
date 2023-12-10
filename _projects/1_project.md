---
layout: page
title: NST for histology
description: An innovative project incorporating Neural Style Transfer concepts for use in histopathology.
img: assets/img/12.jpg
importance: 1
category: work
related_publications: MOGHADAM2022105219, zingman2023comparative
---

The Virtual Stain Transfer for Histopathology project exhibits the integration of Neural Style Transfer (NST) with histopathology. NST allows the re-styling of images to mimic the stylistic elements of a reference image. When applied to histopathology, it can potentially improve diagnostic capabilities, as discussed in \cite{MOGHADAM2022105219} and \cite{zingman2023comparative}.

The project involves the utilization of both supervised and unsupervised learning, the former employing UNets training on around 7,500 images. The use of losses such as Kullback-Leibler Divergence (KLD) and weighted Mean Square Error (MSE) are implemented during the training phase. The project data includes large 3D datasets (&sim;250 GB), where chunking and normalization techniques were experimented on that led to a 10% improvement in the training loss.

On the unsupervised front, Generative Adversarial Networks (GANs) were employed, leveraging algorithms like Pix2Pix and CycleGAN. It's noteworthy that these unsupervised methods outperformed the supervised method by almost 15% on a validation set of 750 images.
  
This project showcases the potential of combining machine learning techniques with medical science for improved disease diagnosis and understanding.

{% include figure.html path="assets/img/12.jpg" title="CycleGAN" class="img-fluid rounded z-depth-1" %}

Developer's notes: This project was a challenging yet enlightening journey into the depth of Neural Style Transfer applications to medical science. It underlines the immense possibilities that lay ahead in this exciting intersection of technology and healthcare.