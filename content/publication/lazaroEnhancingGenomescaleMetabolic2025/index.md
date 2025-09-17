---
title: "Enhancing genome-scale metabolic models with kinetic data: resolving growth and citramalate production trade-offs in Escherichia coli"
authors:
- Jorge Lázaro
- admin
- Jorge Júlvez
- Stephen G. Oliver
date: "2025-07-12T00:00:00Z"

# Schedule page publish date (NOT publication's date).
publishDate: "2025-07-13T00:00:00Z"

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ["article-journal"]

# Publication name and optional abbreviated publication name.
publication: "Bioinformatics Advances"
publication_short: "Bioinf Adv"

abstract: Metabolic models are valuable tools for analyzing and predicting cellular features such as growth, gene essentiality, and product formation. Among the various types of metabolic models, two prominent categories are constraint-based models and kinetic models. Constraint-based models typically represent a large subset of an organism's metabolic reactions and incorporate reaction stoichiometry, gene regulation, and constant flux bounds. However, their analyses are restricted to steady-state conditions, making it difficult to optimize competing objective functions. In contrast, kinetic models offer detailed kinetic information but are limited to a smaller subset of metabolic reactions, providing precise predictions for only a fraction of an organism's metabolism. To address these limitations, we proposed a hybrid approach that integrates these modeling frameworks by redefining the flux bounds in genome-scale constraint-based models using kinetic data. We applied this method to the constraint-based model of _Escherichia coli_, examining both its wild-type form and a genetically modified strain engineered for citramalate production. Our results demonstrate that the enriched model achieves more realistic reaction flux boundaries. Furthermore, by fixing the growth rate to a value derived from kinetic information, we resolved a flux bifurcation between growth and citramalate production in the modified strain, enabling accurate predictions of citramalate production rates.

# Summary. An optional shortened abstract.
summary: ""

tags:
- Metabolism
- Metabolic modelling
featured: false

hugoblox:
  ids:
    doi: 10.1093/bioadv/vbaf166

links:
  - type: pdf
    url: https://academic.oup.com/bioinformaticsadvances/article-pdf/5/1/vbaf166/63735660/vbaf166.pdf
  - type: code
    url: https://github.com/jlazaroibanezz/citrabounds
#  - type: dataset
#    url: ""
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
  caption: 'Image credit: [Amy Karle](https://commons.wikimedia.org/wiki/File:Bioart_in_bio_atelier_at_Mori_Art_Museum_(artwork_by_Amy_Karle).jpg)'
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
A common way to simulate metabolism in an organism is by metabolic models -- mathematical equations that describe the dynamics of chemical reactions. Genome-scale constraint-based metabolic models account for most reactions that can occur in a cell and can be used to predict how much a genetically engineered microbe can produce an industrially relevant compound.

However, a common method to simulate constraint-based metabolic models forces cellular reactions to either be optimised only for growth or only for production of the new compound -- neither of which is realistic. We solve this problem for _E. coli_ producing citramalate by using information from another type of metabolic model to constrain the reaction fluxes in the base constraint-based model for _E. coli_. 
