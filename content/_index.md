---
# Leave the homepage title empty to use the site title
title: ""
date: 2022-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: resume-biography-3
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      text: ""
      # Show a call-to-action button under your biography? (optional)
      button:
        text: Download CV
        url: uploads/resume.pdf
    design:
      css_class: dark
      # Avatar customization
      avatar:
        size: medium  # Options: small (150px), medium (200px, default), large (320px), xl (400px), xxl (500px)
        shape: circle # Options: circle (default), square, rounded
      background:
        color: black
        image:
          # Add your image background to `assets/media/`.
          filename: stacked-peaks.svg
          filters:
            brightness: 1.0
          size: cover
          position: center
          parallax: false
  - block: markdown
    content:
      title: '📚 My Research'
      subtitle: ''
      text: |-
        I am a postdoctoral researcher at the Mahidol-Oxford Tropical Medicine Research Unit (MORU), working with [Dr Claire Chewapreecha](https://www.tropmedres.ac/team/claire-chewapreecha) and [Dr Emma Davenport](https://davenportlab.com/) at the [Wellcome Sanger Institute](https://www.sanger.ac.uk/) to find the transcriptomic and genetic basis for the host-pathogen interaction of melioidosis which determines severe disease. Melioidosis is a neglected tropical disease, endemic to areas such as Northeastern Thailand and Northern Australia.

        My further research interests include risk modelling and disease surveillance, including genomic surveillance, and how this fits in with public health, policy, and media. I'm also interested in best practices in developing software for biomedical research. My geek interests includes Linux and [GNU Emacs](https://www.gnu.org/software/emacs/). [Doom Emacs](https://github.com/doomemacs/doomemacs) is responsible for a lot of my life, including writing my thesis and this website.
        
        Previously, my PhD at the University of Edinburgh was jointly supervised by [Dr Diego Oyarzún](https://homepages.inf.ed.ac.uk/doyarzun/) and [Prof Peter Swain](https://swainlab.bio.ed.ac.uk/). My project examined the metabolic oscillations in budding yeast using single-cell microfluidics.
    design:
      columns: '1'
  - block: collection
    id: papers
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      view: article-grid
      columns: 2
  - block: collection
    content:
      title: Recent Publications
      text: ""
      filters:
        folders:
          - publication
        exclude_featured: false
    design:
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      view: article-grid
      columns: 1
  - block: collection
    id: news
    content:
      title: Recent News
      subtitle: ''
      text: ''
      # Page type to display. E.g. post, talk, publication...
      page_type: post
      # Choose how many pages you would like to display (0 = all pages)
      count: 5
      # Filter on criteria
      filters:
        author: ""
        category: ""
        tag: ""
        exclude_featured: false
        exclude_future: false
        exclude_past: false
        publication_type: ""
      # Choose how many pages you would like to offset by
      offset: 0
      # Page order: descending (desc) or ascending (asc) date.
      order: desc
    design:
      # Choose a layout view
      view: date-title-summary
      # Reduce spacing
      spacing:
        padding: [0, 0, 0, 0]
  - block: cta-card
    demo: true # Only display this section in the Hugo Blox Builder demo site
    content:
      title: 
      text: |-
        .
      button:
        text: .
        url: https://hugoblox.com/templates/
    design:
      card:
        # Card background color (CSS class)
        css_class: "bg-primary-700"
        css_style: ""
---
