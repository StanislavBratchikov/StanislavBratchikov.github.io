---
title: <span style="color:blue; text-decoration:underline;">Predicting Pneumonia Outcomes: Deep Learning and Traditional Methods</span>
summary: Employment of advanced deep learning methods and traditional approaches to identify key factors in predicting clinical outcomes for severe pneumonia patients  using diverse patient data, including single-cell RNAseq and electronic health records from large-scale NIAID-funded study.
tags: 
  - SC RNAseq
date: "2023-09-01T00:00:00Z"

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
url_slides: 
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

***Background:*** <br>Large scale NIAID funded study *Successful Clinical Response In Pneumonia Treatment* of hospitalized patients with severe pneuomina held across several years at Northwestern Memorial Hospital is collecting multiple types of patients data including: *Single cell RNAseq*, *flow cytometry of broncheoalveolar lavage fluid*, *cytokines abundance information*, *electronic health records* that include many clinical and biological factors such as *gender* of patient or *days since intubation* of patient in icu. This data might be useful when answering following questions: 
* Is immune response to various pathogens pre-programmed or adaptive?
* Dependence of the response from secondary/primary infection?
* Can we predict ventilator acquired pneumonia onset within the next 7 days in intensive care unit?
* Can we predict ventilator acquired pneumonia outcome?
* How do long COVID patients stratify/cluster based on scRNA-seq?

Recent advances in biomedical deep learning introduced several useful tools for exploring and integrating multimodal biological data. These tools can be used to address questions above.<br>
***Methods:*** <br>We have collected a diverse dataset of 1741 samples generated from bronchoalveolar lavage fluid of patients with lung diseases and samples from healthy volunteers. For 263 samples additional single cell RNASeq data was provided. Several Deep Learning methods were selected for *healthy* vs *SARS-Cov2* conditions comparison: including [factor decomposition methods](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6010767/),[laten pertubation methods](https://www.nature.com/articles/s41592-023-01969-x), [single cell large language models](https://www.nature.com/articles/s41586-023-06139-9). These methods were used to discover gene expression patterns between different conditions to identify genetic drivers of researched diseases. In order to fine-tune discussed models and make sense of results they produce a comparison benchmark was introduced.<br>
***Results:*** <br>I have performed [state-of-the-art](https://doi.org/10.1038/s41467-021-25960-2) differential gene expression analysis using pseudobulk subsampling technique. Produced sets of genes that differed between conditions were used for models benchamarking. Finally, I have trained a gradient boosting based model to select most informative deep learning method for predicting clinical outcome of patient.<br>
***Conclusions:*** <br>We present a comprehensive study of severe-pneumonia patients using deep learning and traditional methods.Using clinical samples acquired in translational research settings we have identified most informative methods when predicting ventilator pneumonia onset, acquiring pathogen associations with clinical outcomes and determine pathogen-associated immune response.



