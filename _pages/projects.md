---
layout: page
title: Projects
permalink: /projects/
description: A growing collection of your cool projects.
nav: true
nav_order: 2
display_categories: [work, fun]
horizontal: false
---

<!-- pages/projects.md -->
<div class="projects">
{% if site.enable_project_categories and page.display_categories %}
  <!-- Display categorized projects -->
  {% for category in page.display_categories %}
  <h2 class="category">{{ category }}</h2>
    {% assign categorized_projects = site.projects | where: "category", category %}
    {% assign sorted_projects = categorized_projects | sort: "importance" %}
    <!-- Generate cards for each project -->
    {% if page.horizontal %}
    <div class="container">
      <div class="row row-cols-2">
      {% for project in sorted_projects %}
        <h3>Alpenglow Biosciences</h3>
        <p>Deep Learning Research Intern: Worked on stain transfer problem and optimized data processing pipeline, amongst other tasks.</p>
        <h3>RadiusAI</h3>
        <p>Computer Vision Researcher (Capstone): Worked on self-checkout problem using synthetic Image Generation to improve training of object detection models.</p>
        <h3>GRAIL: UW Graphics and Imaging Laboratory</h3>
        <p>Graduate Research Assistant: Developed vision-language histopathology dataset and designed a neural network.</p>
        <h3>Indian Institute of Science, Bangalore</h3>
        <p>Bachelor Thesis: Worked on optimizing the performance of GANs and Wasserstein Generative Adversarial Networks.</p>
        <h3>Peter L. Reichertz Institute for Medical Informatics - TU Braunschweig</h3>
        <p>Research Intern: Performed Blood Pressure estimation from photoplethysmogram signals.</p>
        <h3>Centre for Computational Imaging - IIT Palakkad</h3>
        <p>Summer Research Intern: Analysed Subtle Motion on ultrasound images of the Common Carotid Artery.</p>
      {% endfor %}
      </div>
    </div>
  {% else %}
  <div class="grid">
    {% for project in sorted_projects %}
      {% include projects.html %}
    {% endfor %}
  </div>
  {% endif %}
  {% endfor %}

{% else %}
<!-- Display projects without categories -->
  {% assign sorted_projects = site.projects | sort: "importance" %}
  {% if page.horizontal %}
  <div class="container">
    <div class="row row-cols-2">
    {% for project in sorted_projects %}
      {% include projects_horizontal.html %}
    {% endfor %}
    </div>
  </div>
  {% else %}
  <div class="grid">
    {% for project in sorted_projects %}
      {% include projects.html %}
    {% endfor %}
  </div>
  {% endif %}
{% endif %}
</div>