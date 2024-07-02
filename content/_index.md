---
# Leave the homepage title empty to use the site title
title: svdg
date: 2023-04-17
type: landing

sections:
  - block: about.avatar
    id: about
    content:
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
      # Override your bio text from `authors/admin/_index.md`?
      text:
  - block: markdown
    id: publications
    content:
      title: Publications
      subtitle: 
      text: 
  - block: collection
    id: preprints
#    id: publications
    content:
      title: Preprints
      filters:
        # Folders to display content from
        folders:
          - publication
        publication_type: "3"
      count: 0
      archive:
        enable: false
    # Field to sort by, such as Date or Title
      sort_by: 'Date'
      sort_ascending: false
    design:
      columns: '2'
      view: citation
  - block: collection
    content:
      title: Reviewed
      filters:
        folders:
          - publication
#        exclude_featured: true
        publication_type: "2"
      count: 0
      archive:
        enable: false
    design:
      columns: '2'
      view: citation
  - block: collection
    content:
      title: Other Publications
      filters:
        folders:
          - publication
        publication_type: "0"
      count: 0
      archive:
        enable: false
    design:
      columns: '2'
      view: citation
  - block: collection
    content:
      title: Thesis
      filters:
        folders:
          - publication
        publication_type: "7"
    design:
      columns: '2'
      view: list
  - block: markdown
    id: events
    content:
      title: Upcoming Events
      subtitle: 
      text: 
  - block: collection
    id: # events
    content:
      title: # Upcoming Events
      filters:
        folders:
          - event
      sort_by: 'Date'
      sort_ascending: true
    design:
      columns: '2'
      view: compact
  - block: markdown
    id: projects
    content:
      title: Projects
      subtitle: 
      text: 
  - block: portfolio
    id: # projects
    content:
      title: # Projects
      filters:
        folders:
          - project
        exclude_category: "teaching"
#      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
#      default_button_index: 0
#      # Filter toolbar (optional).
#      # Add or remove as many filters (`filter_button` instances) as you like.
#      # To show all items, set `tag` to "*".
#      # To filter by a specific tag, set `tag` to an existing tag name.
#      # To remove the toolbar, delete the entire `filter_button` block.
#      buttons:
#        - name: All
#          tag: '*'
#        - name: Deep Learning
#          tag: Deep Learning
#        - name: Other
#          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '2'
      view: card # showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    id: teaching
    content:
      title: Teaching
      subtitle: 
      text: 
  - block: collection
    id: # teaching
    content:
      title: # teaching
      filters:
        folders:
          - project
        exclude_category: "teaching"
      sort_by: 'Date'
      sort_ascending: true
    design:
      columns: '2'
      view: compact
  - block: markdown
    id: contact
    content:
      title: Contact
      subtitle: 
      text: 
  - block: contact
    id: # contact
    content:
      title: # Contact
      subtitle:
      text: 
      # Contact (add or remove contact options as necessary)
      email: soeren.von.der.gracht@uni-paderborn.de
      phone: +49 5251 60-3774
#      appointment_url: 'https://calendly.com'
      address:
        street: Technologiepark 21
        city: Paderborn
      #  region: CA
        postcode: '33100'
        country: Germany
        country_code: D
      directions: Office TP21.1.17
#      office_hours:
#        - 'Monday 10:00 to 13:00'
#        - 'Wednesday 09:00 to 10:00'
#      contact_links:
#        - icon: twitter
#          icon_pack: fab
#          name: DM Me
#          link: 'https://twitter.com/Twitter'
#        - icon: skype
#          icon_pack: fab
#          name: Skype Me
#          link: 'skype:echo123?call'
#        - icon: video
#          icon_pack: fas
#          name: Zoom Me
#          link: 'https://zoom.com'
      coordinates:
        latitude: '51.70094721497175'
        longitude: '8.765041497345752'
      # Automatically link email and phone or display as text?
      autolink: true
#      # Email form provider
#      form:
#        provider: netlify
#        formspree:
#          id:
#        netlify:
#          # Enable CAPTCHA challenge to reduce spam?
#          captcha: false
    design:
      columns: '2'
#  - block: experience
#    id: experience
#    content:
#      title: Experience
#      # Date format for experience
#      #   Refer to https://wowchemy.com/docs/customization/#date-format
#      date_format: Jan 2006
#      # Experiences.
#      #   Add/remove as many `experience` items below as you like.
#      #   Required fields are `title`, `company`, and `date_start`.
#      #   Leave `date_end` empty if it's your current employer.
#      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
#      items:
#        - title: CEO
#          company: GenCoin
#          company_url: ''
#          company_logo: org-gc
#          location: California
#          date_start: '2021-01-01'
#          date_end: ''
#          description: |2-
#              Responsibilities include:
#
#              * Analysing
#              * Modelling
#              * Deploying
#        - title: Professor of Semiconductor Physics
#          company: University X
#          company_url: ''
#          company_logo: org-x
#          location: California
#          date_start: '2016-01-01'
#          date_end: '2020-12-31'
#          description: Taught electronic engineering and researched semiconductor physics.
#    design:
#      columns: '2'
#  - block: accomplishments
#    content:
#      # Note: `&shy;` is used to add a 'soft' hyphen in a long heading.
#      title: 'Accomplish&shy;ments'
#      subtitle:
#      # Date format: https://wowchemy.com/docs/customization/#date-format
#      date_format: Jan 2006
#      # Accomplishments.
#      #   Add/remove as many `item` blocks below as you like.
#      #   `title`, `organization`, and `date_start` are the required parameters.
#      #   Leave other parameters empty if not required.
#      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
#      items:
#        - certificate_url: https://www.coursera.org
#          date_end: ''
#          date_start: '2021-01-25'
#          description: ''
#          organization: Coursera
#          organization_url: https://www.coursera.org
#          title: Neural Networks and Deep Learning
#          url: ''
#        - certificate_url: https://www.edx.org
#          date_end: ''
#          date_start: '2021-01-01'
#          description: Formulated informed blockchain models, hypotheses, and use cases.
#          organization: edX
#          organization_url: https://www.edx.org
#          title: Blockchain Fundamentals
#          url: https://www.edx.org/professional-certificate/uc-berkeleyx-blockchain-fundamentals
#        - certificate_url: https://www.datacamp.com
#          date_end: '2020-12-21'
#          date_start: '2020-07-01'
#          description: ''
#          organization: DataCamp
#          organization_url: https://www.datacamp.com
#          title: 'Object-Oriented Programming in R'
#          url: ''
#    design:
#      columns: '2'
#  - block: tag_cloud
#    content:
#      title: Popular Topics
#    design:
#      columns: '2'
---
