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
        url: uploads/Joe_Pappas_CV_5_27.pdf
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
      title: 'About Me'
      subtitle: ''
      text: |-
        I'm driven by a profound passion for enabling farmers to sustainably meet the escalating demands of our rapidly expanding world. Specializing in machine learning, I am constantly exploring innovative avenues to synergize my expertise with this fervent commitment. I am looking for Robotics companies in the agriculture space to improve their Computer Vision subsystems.

        I received my Bachelor of Science degree from Ohio State University, majoring in Computer Science and Engineering with a focus in Artificial Intelligence. My interests and course work included basic and advanced AI Techniques, Machine Learning and Statistical Pattern Recognition, and Neural Networks. 

        I started my Master's degree in August of 2022 as a Research Assistant with Fellowship at Purdue University in the school of Agricultural and Biological Engineering under Professor Somali Chaterji in her ICAN Lab. My current work includes mobile GPU resource optimization, optimal UAV (drone) deployment strategies for the tradeoff between detection quality, latency and area coverage, and cloud database optimization. We are focused on optimizing Machine Learning models at the edge for use in robotics systems.
    design:
      columns: '1'
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
        featured_only: true
    design:
      view: article-grid
      columns: 1
---
