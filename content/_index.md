---
# Leave the homepage title empty to use the site title
title: "Arnab's webpage"
date: 2025-10-18
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
        <div align="center">
        Hello! I'm a researcher working in the field of neutrino physics and beyond the Standard Model physics. My research primarily focuses on understanding the fundamental properties of neutrinos and          probing possible new physics effects through phenomenological studies. I am also actively involved in the application of machine learning techniques to high-energy physics, with the goal of               enhancing event reconstruction, parameter estimation, and sensitivity studies in neutrino experiments.
        I am always open to discussions and collaborations in related areas of high energy physics.
        <div>
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
      columns: 3
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
---
