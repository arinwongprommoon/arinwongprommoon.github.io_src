---
title: PhD Project
summary: PhD Project 
tags:
  - Microfluidics
  - Live-cell imaging
  - Yeast
  - Metabolism
  - Metabolic modelling
  - Machine Learning
  - Time series analysis
  - Software development
date: '2019-10-01T00:00:00Z'

# Optional external URL for project (replaces project detail page).
external_link: ''

image:
  caption: Photo by rawpixel on Unsplash
  focal_point: Smart

links:
#  - icon: twitter
#    icon_pack: fab
#    name: Follow
#    url: https://twitter.com/georgecushen
url_code: ''
url_pdf: ''
url_slides: ''
url_video: ''

# Slides (optional).
#   Associate this project with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides = "example-slides"` references `content/slides/example-slides.md`.
#   Otherwise, set `slides = ""`.
slides: 
---

My PhD project is conducted under the joint jointly supervision by [Dr Diego Oyarzún](https://homepages.inf.ed.ac.uk/doyarzun/) (computational) and [Prof Peter Swain](https://swainlab.bio.ed.ac.uk/) (laboratory & computational), at the University of Edinburgh.

My project examines the metabolic cycle in budding yeast. This yeast metabolic cycle is defined by levels of metabolites in the cell increasing and decreasing in regular cycles, which are linked to cell division. Changing feeding conditions for the yeast cells or removing genes from the yeast genome that are responsible for metabolic processes affect the speed of these metabolic cycles.

Not a lot of people study this cycle. Those who do study them in chemostats -- essentially, large liquid cultures of many cells -- so it is difficult to see whether individual cells behave differently. This is why I use microfluidics to separate the cells. Microfluidics refers to an experimental system that moves around small amounts of liquids -- in my case, I use microfluidics to move cells from cultures, trap & separate them, then add or remove nutrients over time.

Over time, my project has matured into three parts:

1. _Find out ways to analyse the thousands of oscillatory time series I produce._ Microfluidics is nice because I get data from many cells. But then I have to clean, process, and categorise this data. I also find out that commonly-used computational methods to compute the periodicity of data, such as the Fourier transform, do not work so well with the noisy biological data I have. My aim is then to find alternative methods, and combine them with other data-processing steps in a data analysis pipeline. In [this code repository](https://github.com/arinwongprommoon/phd-synthetic-oscillations), I investigate how noise in the data affect some analysis methods. And [here is a work-in-progress repository](https://github.com/arinwongprommoon/phd-classifier) of trying to use machine learning to tell apart oscillatory and non-oscillatory signals.
2. _Show that the metabolic cycle occurs in a variety of cell conditions._ My hypothesis here is that the metabolic cycle is something fundamental in the yeast cell, therefore I should be able to see oscillations in metabolite levels when the cells have certain genes removed, or are starved of nutrients. So far, so good. [Here is a jumble of code](https://github.com/arinwongprommoon/phd-ymc-dataviz) that I use to process the data I obtain from my microfluidics experiments to produce reports of the cells in each experiment.
3. _Use mathematical models of metabolism to explain why yeast cells have these metabolic cycles._ More specifically, I answer the question: does it make sense for the cell to make different building blocks (carbohydrates, proteins, fats) at different times, and do these times fit with the periodicity of the metabolic cycle that I observe in experiments? To do this, I use a genome-scale metabolic model -- essentially, a list of chemical reactions that can happen in the yeast cell -- and solve linear programming problems to see how fast each reaction should be so that the cell grows as fast as possible. [Here is the code](https://git.ecdf.ed.ac.uk/s1947236/fba-temporal-biosynthesis) that I use to solve these problems.

In addition, I was part of the team that developed [aliby](https://pypi.org/project/aliby/), a Python-based pipeline that Peter Swain's research group uses to analyse time-lapses of images of yeast cells taken from the microscopes in their microfluidics systems. This pipeline finds cells in the images (segmentation), keeps track of cells as they move through time (tracking), match new cells to the ones they divided from (lineage prediction), and creates time series for further processing. I use this software extensively in part 2 of my project.

For me, this was a valuable foray in collaborative software development. Of course, I sharpened my Python skills, but also DevOps: automated testing and deployment of software, managing software versions, maintaining servers for users, and making sure things don't crash and burn. I learnt how to talk to other developers, project managers, and users (biologist and physicists) of varying programming or technical abilities. Naturally, I learnt to navigate lots and lots and lots of conflicts -- both merge conflicts and inevitable conflicts between people!

My PhD work eventually led to a paper that showed that [single-cell metabolic oscillations are pervasive and may alleviate a proteome constraint]({{< relref "../../publication/wongprommoonSinglecellMetabolicOscillations/" >}}). During my PhD, I also worked on a paper on the [accuracy and data efficiency in deep learning models of protein expression]({{< relref "../../publication/nikoladosaccuracydataefficiency2022/" >}}).
