---
title: Flow Cytometry
summary: A machine learning classifier trained on 172 expert-annotated clinical flow cytometry samples, achieving accurate cell typing, overcoming biases, and scaling to over 1100 samples, demonstrating high accuracy and significant time savings.
tags:
  - Flow Cytometry
date: ''

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: ''
  focal_point: Smart

links:
  - icon: twitter
    icon_pack: fab
    name: Follow
    url: https://twitter.com/brtchkvs
url_code: ''
url_pdf: ''
url_slides: https://docs.google.com/presentation/d/10BWF-NMwT0HdYpbd-NxwFP6GKXvv9o0qpw4vTQvvwDQ/edit?usp=sharing
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

***Background:*** Multiparameter flow cytometry is an invaluable tool for translational research which provides in depth immunophenotyping of the clinical samples. Traditionally, analysis of the flow cytometry data is performed manually by experts who have to take into account both technical and biological variability. This approach is prone to expert-specific biases and does not scale to hundreds of samples. We hypothesize that a machine learning classifier can be applied to clinical flow cytometry samples and can achieve cell typing accuracy comparable to expert annotations, overcome technical variability while preserving biological variability, and scale up to hundreds of clinical samples.<br>
***Methods:*** We have generated a diverse set of 172 expert-annotated clinical flow cytometry samples generated from bronchoalveolar lavage fluid from patients with lung diseases, including severe pneumonia, respiratory PASC, samples from lung transplant patients, and samples from healthy volunteers. We split this dataset with a 7:3 train-validation ratio to train and optimize a model based on a gradient boosting LightGBM classifier. We have validated our model using previously annotated external dataset of hundreds of clinical samples from patients with lung diseases.<br>
***Results:*** After hyperparameter optimization our model achieved high classification accuracy for both common and rare cell types. Our model performed well on phenotypically distinct cell types (such as T cell subsets) or phenotypically plastic cell types (such as neutrophils and macrophages), thus, preserving biological variability. The model performed well when it was applied to a large (>1100 samples) clinical datasets from multiple studies. Our model required only ~1 second per sample, which saves about 4 mins of expert’s time for every sample.<br>
***Conclusions:*** We present a scalable and generalizable approach for rapid and accurate annotation of clinical samples acquired in translational research settings. Our approach addresses many issues inherent to analysis of clinical flow cytometry samples and increases reproducibility.


