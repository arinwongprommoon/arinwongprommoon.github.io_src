---
title: "Accuracy and data efficiency in deep learning models of protein expression"
authors:
- Evangelos-Marios Nikolados
- admin
- Oisin Mac Aodha
- Guillaume Cambray
- Diego A. Oyarzún 
date: "2022-12-15T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-01-01T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "Nature Communications"
publication_short: "Nat Commun"

abstract: Synthetic biology often involves engineering microbial strains to express high-value proteins. Thanks to progress in rapid DNA synthesis and sequencing, deep learning has emerged as a promising approach to build sequence-to-expression models for strain optimization. But such models need large and costly training data that create steep entry barriers for many laboratories. Here we study the relation between accuracy and data efficiency in an atlas of machine learning models trained on datasets of varied size and sequence diversity. We show that deep learning can achieve good prediction accuracy with much smaller datasets than previously thought. We demonstrate that controlled sequence diversity leads to substantial gains in data efficiency and employed Explainable AI to show that convolutional neural networks can finely discriminate between input DNA sequences. Our results provide guidelines for designing genotype-phenotype screens that balance cost and quality of training data, thus helping promote the wider adoption of deep learning in the biotechnology sector.

# Summary. An optional shortened abstract.
summary: Deep learning, a type of machine learning, can be used to predict how much protein a specific DNA sequence can produce. But, it usually needs a lot of data. We managed to get a deep learning model to do make predictions with less data, especially if the data is diverse. Our study is useful because people can then produce fewer DNA to train a model, and this is cheaper.

tags:
- Machine learning
- Deep learning
- Explainable AI
- Synthetic biology 
featured: false

hugoblox:
  ids:
    doi: 10.1038/s41467-022-34902-5

links:
  - type: pdf
    url: https://www.nature.com/articles/s41467-022-34902-5.pdf 
  - type: code
    url: https://doi.org/10.5281/zenodo.7273952
  - type: dataset
    url: https://doi.org/10.5281/zenodo.7273952
#  - type: poster
#    url: ""
#  - type: project
#    url: ""
#  - type: slides
#    url: ""
#  - type: source
#    url: ""
#  - type: video
#    url: ""

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [Nikolados et al.]'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

## Lay summary
Deep learning, a type of machine learning, can be used to predict how much protein a specific DNA sequence can produce. But, it usually needs a lot of data.

We managed to get a deep learning model to make predictions with less data, especially if the data is diverse.

Our study is useful because people can then produce fewer DNA to train a model, and this is cheaper.

## My role
I made sure that the Python code for the non-deep and deep learning models was robust and easy for people to use.

I also gave feedback on the manuscript. My comments improved a figure; it shows that a diverse DNA sequence input improved how efficiently the model worked and how much it was able to handle a variety of sequences.
