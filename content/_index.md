---
date: "2022-10-24"
sections:
- block: about.avatar
  content:
    text: null
    username: admin
    columns: 1
  id: about
#- block: experience
#  content:
#    date_format: Jan 2006
#    items:
#    - company: GenCoin
#      company_logo: org-gc
#      company_url: ""
#      date_end: ""
#      date_start: "2021-01-01"
#      description: |2-
#          Responsibilities include:
#
#          * Analysing
#          * Modelling
#          * Deploying
#      location: California
#      title: CEO
#    - company: University X
#      company_logo: org-x
#      company_url: ""
#      date_end: "2020-12-31"
#      date_start: "2016-01-01"
#      description: Taught electronic engineering and researched semiconductor physics.
#      location: California
#      title: Professor of Semiconductor Physics
#    title: Experience
#  design:
#    columns: "2"
#- block: collection
#  content:
#    count: 5
#    filters:
#      author: ""
#      category: ""
#      exclude_featured: false
#      exclude_future: false
#      exclude_past: false
#      folders:
#      - post
#      publication_type: ""
#      tag: ""
#    offset: 0
#    order: desc
#    subtitle: ""
#    text: ""
#    title: Recent Posts
#  design:
#    columns: "2"
#    view: compact
#  id: posts
- block: portfolio
  content:
    buttons:
    - name: All
      tag: '*'
    - name: Shape Constraint Inference 
      tag: Shape Constraint Inference
    - name: Other
      tag: Demo
    default_button_index: 0
    filters:
      folders:
      - project
    title: Projects
  design:
    columns: "1"
    flip_alt_rows: false
    view: showcase
  id: projects
#- block: markdown
#  content:
#    subtitle: ""
#    text: '{{< gallery album="demo" >}}'
#    title: Gallery
#  design:
#    columns: "1"
#- block: collection
#  content:
#    filters:
#      featured_only: true
#      folders:
#      - publication
#    title: Featured Publications
#  design:
#    columns: "2"
#    view: card
#  id: featured
- block: collection
  content:
    filters:
      exclude_featured: true
      folders:
      - publication
    title: Recent Publications
  design:
    columns: "2"
    view: citation
  id: publications
#- block: collection
#  content:
#    filters:
#      folders:
#      - event
#    title: Recent & Upcoming Talks
#  design:
#    columns: "2"
#    view: compact
#  id: talks
#- block: tag_cloud
#  content:
#    title: Popular Topics
#  design:
#    columns: "2"
- block: contact
  content:
    #address:
    #  city: Stanford
    #  country: United States
    #  country_code: US
    #  postcode: "94305"
    #  region: CA
    #  street: 450 Serra Mall
    #appointment_url: https://calendly.com
    #autolink: true
    #contact_links:
    #- icon: twitter
    #  icon_pack: fab
    #  link: https://twitter.com/Twitter
    #  name: DM Me
    #- icon: skype
    #  icon_pack: fab
    #  link: skype:echo123?call
    #  name: Skype Me
    #- icon: video
    #  icon_pack: fas
    #  link: https://zoom.com
    #  name: Zoom Me
    directions: Mekelweg 4, 2628 CD Delft, NL. Office HB06.032.
    email: f.gili@tudelft.nl
    office_hours: Contact me for office hours, or schedule an appointment.
    #phone: 888 888 88 88
    #subtitle: null
    #text: Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nam mi diam, venenatis
    #  ut magna et, vehicula efficitur enim.
    title: Contact
  design:
    columns: "2"
  id: contact
title: null
type: landing
---
