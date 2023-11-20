---
title: 'Developing pipeline for single cell spatial transcriptomics analysis'
summary: Exploring single cell spatial transcriptomics, the study compared 10x Xenium and Nanostring CosMx, using Python and R tools to assess their applicability in the laboratory based on factors such as transcript coverage and specificity as well as ability to preserve biological variation.
tags: 
  - SC RNAseq
date: "2023-08-01T00:00:00Z"

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
url_slides: https://docs.google.com/presentation/d/1l1zRh1nwhJxOKwIodAbxsXKHls5V1DgyfBAeG93__zI/edit?usp=sharing
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: ""
---

***Background:*** <br>Single cell spatial transcriptomics is a rapidly developing area in the field of sc RNAseq. Unlike spot-based spatial transcriptomics, single cell spatial transcriptomics can provide cellular and even subcellular resolution. Information about spatial coordinates of RNA transcripts within cell and globally in tissue can provide critical insights about its structure and function. Multiple companies have tried to fill this niche of research and provide commercially available platform for performing this sequencing. List of popular commercially available platforms include: [10x Xenium](https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwjo89i7rtGCAxUv9cgKHctzDKoYABABGgJxdQ&ae=2&gclid=CjwKCAiAgeeqBhBAEiwAoDDhn_S6tNz4HIH04-_2MrRSqsZfbgMPJp6YO1REejhqkcK2ZYGwuV69ZBoCaowQAvD_BwE&ohost=www.google.com&cid=CAESVeD26pbz1L-HRB1hXq_OG-qwGCxIAHcrT8XnwT-tcDS_iS619GcpRvo1baDpJEpWrGxuK3C_jQHvSoQjIprfYcPwi9owNTwLe3xgYoC2hUpNXrMEC4Q&sig=AOD64_0zFm8OkHVcIVqflExyqP8gcN-HbQ&q&adurl&ved=2ahUKEwiilNG7rtGCAxUYhIkEHTmgBEMQ0Qx6BAgNEAE&nis=2&dct=1), [Nanostring CosMx](https://www.googleadservices.com/pagead/aclk?sa=L&ai=DChcSEwiCs5_VrtGCAxWDRnIKHebfAN0YABAAGgJxdQ&ae=2&gclid=CjwKCAiAgeeqBhBAEiwAoDDhn2XjeHBaNMp-kMSqSNiggx491ZiVasgR9IvjNVfNYRTFL8z027aNxRoCaAcQAvD_BwE&ohost=www.google.com&cid=CAESVeD2UbO_fHyW6KtkY3QlIdo5k5yzZFi_m9R3SwoyXre3dzfdAWj5WIu0J7RS_Nj5TgoC-V3QRf9H5CLMVYH168kB9JOc0HfGlIQP6rewb5PxkJvqxPE&sig=AOD64_3MunaYXo8FTaRC_SHzEXG0Sk10-Q&q&adurl&ved=2ahUKEwjG3ZnVrtGCAxX0pIkEHQZICTYQ0Qx6BAgKEAE&nis=2&dct=1), and [Vizgen MERFISH](https://www.google.com/url?sa=t&rct=j&q=&esrc=s&source=web&cd=&cad=rja&uact=8&ved=2ahUKEwiygtGfrtGCAxWvAHkGHU4KAJAQFnoECC8QAQ&url=https%3A%2F%2Fvizgen.com%2F&usg=AOvVaw0qedZkpasuzvGnXLTb3d9a&opi=89978449).<br>
***Methods:*** <br>We have researched publicly available datasets and our own in-house data to compare CosMx and Xenium. For this purpose we used currently available analysis tools using python and R packages: ```Squidpy```,```Giotto```,```stLearn```, ```Spapros``` and ```Seurat```. <br>
***Results:*** <br>I have compared coverage of RNA transcripts within given samples to find platform that provides the best transcript coverage. Additionaly I have estimated experiment and tissue specific batch effects and ways to integrate data preserving biological variability while reducing technical variation. Finally, I have studied multiple tools for targeted gene panel construction used in spatial transcriptomics. These tools allowed selecting 50 additional genes to add to existent commercial gene panels that would best preserve biological variation of human lung tissue.<br>
***Conclusions:*** <br>Based on data used in my comparison, Xenium platform provided better transcript coverage and specificity. Lack of field of view stiching in CosMx produces cell duplications that may influence analysis. This comparison analysis enabled bringing these platforms to our laboratory and provided a standard pipeline for handling spatial transcriptomics data in the laboratory. 




