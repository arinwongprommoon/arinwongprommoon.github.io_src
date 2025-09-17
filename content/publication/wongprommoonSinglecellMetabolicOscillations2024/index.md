---
title: "Single-cell metabolic oscillations are pervasive and may alleviate a proteome constraint"
authors:
- admin
- Alán F. Muñoz
- Diego A. Oyarzún
- Peter S. Swain
date: "2024-11-26T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-11-26T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article"]

# Publication name and optional abbreviated publication name.
publication: "bioRxiv"
publication_short: "bioRxiv"

abstract: "Biological rhythms not only coordinate cellular activity with external signals, but may also enable internal coordination. The metabolic cycle in budding yeast is perhaps the most well-studied example. Historically researchers have investigated this cycle in populations growing in chemostats, but more recently time-lapse microscopy has revealed single-cell oscillations in the redox state of enzyme cofactors and in ATP levels. How to relate the results of these two types of assays is however unclear. Here we report single-cell rhythms too in intracellular pH and show that oscillations in the redox state of flavin molecules occur in auxotrophic and prototrophic strains, in nutrients favouring respiration or fermentation, and in deletion mutants for which oscillations in chemostats are either unobservable or disrupted. To explain the pervasiveness of these rhythms, we postulate that cells generate oscillations to alleviate a proteome constraint -- amino acids cells use for one class of enzymes are unavailable for others. Using flux balance analysis with an enzyme-constrained genome-scale metabolic model, we show that, with a finite proteome, sequential synthesis of biomass components typically generates a shorter doubling time than synthesising components in parallel. Our results suggest that the metabolic cycle drives growth and is potentially widespread because all cells grow within a proteome constraint."

# Summary. An optional shortened abstract.
summary: ""

tags:
  - Microfluidics
  - Live-cell imaging
  - Yeast
  - Metabolism
  - Metabolic modelling
  - Time series analysis
featured: true

hugoblox:
  ids:
    doi: 10.1101/2024.11.25.625147

links:
- type: preprint
  provider: bioRxiv
  url: https://doi.org/10.1101/2024.11.25.625147
- type: code
  url: https://github.com/arinwongprommoon/wongprommoonSinglecellMetabolicOscillations2024
#- type: slides
#  url: https://www.slideshare.net/
- type: dataset
  url: https://doi.org/10.7488/ds/7845
#- type: poster
#  url: "#"
#- type: source
#  url: "#"
#- type: video
#  url: https://youtube.com
#- type: custom
#  label: Custom Link
#  url: http://example.org

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/s9CC2SKySJM)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- [phd]

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---

## Lay summary
Biological rhythms are essential to controlling the function of living organisms. One such example is the metabolic cycle in budding yeast, which consists of cycling levels of metabolites, RNA transcripts, and oxygen consumption over time. Most studies on this cycle have been performed with chemostats, in batch-cultures. Though there are more recent studies that image cells individually, it is unclear how to reconcile finding from the two types of experiments.

In this preprint, we show that pH levels in yeast cells also oscillate along with flavin redox state. These oscillations are present across a greater range of nutrient conditions and yeast mutants than observed before, including conditions in which such oscillations were disrupted in chemostats.

To explain why these oscillations are so prevalent, we used flux balance analysis -- a linear programming-based mathematical method to model biochemical reaction networks. With this tool, we show that, if a cell with a finite level of amino acids makes its biological building blocks (proteins, carbohydrates, lipids, etc.) in sequence, it saves time on growth. Thus, This sequence of synthesis may explain the metabolic oscillations.

## My role
This work represents a fusion of multiple disciplines and tools. To observe the cells, I needed to learn how to use a microfluidics device with so many moving parts. Monitoring cell division was made possible by using CRISPR-Cas9 to engineer a genetic insertion (and I learnt how to do this while social distancing during the COVID-19 pandemic). The time-lapse microscope produces a lot of images, so the research group needed to develop [new software to process them](https://pypi.org/project/aliby/) and I wrote functions to perform time-series analysis. Finally, we used a tool from metabolic engineering, flux balance analysis, to help formulate a theoretical explanation of our observations.

I also co-wrote the initial draft of the manuscript, and documented the datasets and code.
