---
title: "Enhancing the accuracy of genome-scale metabolic models with kinetic information"
authors:
- Jorge Lázaro
- admin
- Jorge Júlvez
- Stephen G. Oliver
date: "2024-07-14T00:00:00Z"
doi: "10.1101/2024.07.11.597182"

# Schedule page publish date (NOT publication's date).
publishDate: "2024-07-15T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["3"]

# Publication name and optional abbreviated publication name.
publication: "bioRxiv"
publication_short: "bioRxiv"

abstract: "Metabolic models can be used to analyze and predict cellular features such as growth estimation, gene essentiality, and product formation. Metabolic models can be divided into two main types: constraint-based models and kinetic models. Constraint-based models usually account for a large subset of the metabolic reactions of the organism and, in addition to the reaction stoichiometry, these models can accommodate gene regulation and constant flux bounds of the reactions. Constraint-based models are mostly limited to the steady state and it is challenging to optimize competing objective functions. On the other hand, kinetic models contain detailed kinetic information of a relatively small subset of metabolic reactions; thus, they can only provide precise predictions of a reduced part of an organism’s metabolism. We propose an approach that combines these two types of models to enrich metabolic genome-scale constraint-based models by re-defining their flux bounds. We apply our approach to the constraint-based model of E. coli, both as a wild-type and when genetically modified to produce citramalate. Consequently, we show that the enriched model has more realistic reaction flux boundaries. We also resolve a bifurcation of fluxes between growth and citramalate production present in the genetically modified model by fixing the growth rate to the value computed according to kinetic information, enabling us to predict the rate of citramalate production."

tags:
- Metabolism
- Metabolic modelling
featured: false

# links:
# - name: "Publication site"
# url: "https://www.biorxiv.org/content/10.1101/2024.07.11.597182v1"
url_pdf: "https://www.biorxiv.org/content/10.1101/2024.07.11.597182v1.full.pdf"
# url_code: ''
# url_dataset: ''
# url_poster: ''
# url_project: ''
# url_slides: ''
# url_source: ''
# url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Image credit: [Philip Patenall/Springer Nature Limited](https://www.nature.com/articles/s41579-024-01033-1)'
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
#slides: example
---

# Lay summary
A common way to simulate metabolism in an organism is by metabolic models -- mathematical equations that describe the dynamics of chemical reactions. Genome-scale constraint-based metabolic models account for most reactions that can occur in a cell and can be used to predict how much a genetically engineered microbe can produce an industrially relevant compound.

However, a common method to simulate constraint-based metabolic models forces cellular reactions to either be optimised only for growth or only for production of the new compound -- neither of which is realistic. We solve this problem for _E. coli_ producing citramalate by using information from another type of metabolic model to constrain the reaction fluxes in the base constraint-based model for _E. coli_. 
