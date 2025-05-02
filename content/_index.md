---
title: 'Home'
date: 2023-10-24
type: landing

design:
  # Default section spacing
  spacing: "6rem"

sections:
  - block: hero
    content:
      title: "SpecFWAT: Illuminate Refined Subsurface Structures"
      text: The easy, fast, and powerful full-waveform adjoint tomography (FWAT) inversion tool for seismic data.
      primary_action:
        text: Clone from GitHub
        url: https://github.com/CompSeismoUT/SpecFWAT
        icon: arrow-down-tray
      secondary_action:
        text: Read the docs
        url: /docs/
      # announcement:
      #   text: "Announcing the release of version 2."
      #   link:
      #     text: "Read more"
      #     url: "/blog/"
    design:
      spacing:
        padding: [0, 0, 0, 0]
        margin: [0, 0, 0, 0]
      # For full-screen, add `min-h-screen` below
      css_class: ""
      background:
        color: ""
        image:
          # Add your image background to `assets/media/`.
          filename: ""
          filters:
            brightness: 0.5
  # - block: stats
  #   content:
  #     items:
  #       - statistic: "1M+"
  #         description: |
  #           Websites built  
  #           with Hugo Blox
  #       - statistic: "10k+"
  #         description: |
  #           GitHub stars  
  #           since 2016
  #       - statistic: "3k+"
  #         description: |
  #           Discord community  
  #           for support
  #   design:
  #     # Section background color (CSS class)
  #     css_class: "bg-gray-100 dark:bg-gray-800"
  #     # Reduce spacing
  #     spacing:
  #       padding: ["1rem", 0, "1rem", 0]
  - block: features
    id: features
    content:
      title: Features
      text: SpecFWAT employ adjoint waveform tomography method and support multiple types of seismic data and is designed to be user-friendly and fast
      items:
        - name: SPECFEM3D
          icon: globe-americas
          description: It is built on top of the open-source software package **[SPECFEM3D](https://specfem.org)** for simulating seismic wave propagation in 3D heterogeneous media.
        - name: Flexible data support
          icon: code-bracket
          description: Teleseismic, ambient noise, and receiver function data are supported and their joint inversion can also be used.
        - name: Multi-parameter inversion
          icon: rectangle-group
          description: Both isotropic and anisotropic elastic parameters can be inverted for.
        - name: Fast
          icon: bolt
          description: Fast and efficient, allowing users to perform FWI on supercomputer accelerated by **GPUs** and **CPUs**.
        - name: Easy
          icon: sparkles
          description: Simple format for model files (**.h5**), data files (**.sac**) and parameter files (**.yml**) that are easy to read and write.
        - name: Scalability
          icon: fortran
          description: It is designed to be scalable under Object-Oriented Fortran by modularizing the code and using CMake for building.
    design:
      # Section background color (CSS class)
      css_class: "bg-gray-100 dark:bg-gray-800"
      # Reduce spacing
      spacing:
        padding: ["1rem", 0, "1rem", 0]
  # - block: cta-card
  #   content:
  #     title: "Start Writing with the #1 Effortless Documentation Platform"
  #     text: Hugo Blox Docs Theme brings all your technical knowledge together in a single, centralized knowledge base. Easily search and edit it with the tools you use every day!
  #     button:
  #       text: Get Started
  #       url: https://hugoblox.com/templates/details/docs/
  #   design:
  #     card:
  #       # Card background color (CSS class)
  #       css_class: "bg-primary-700"
  #       css_style: ""
---
