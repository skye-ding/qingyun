---
# Leave the homepage title empty to use the site title
title:
date: 2022-10-24
type: landing

sections:
  - block: about.biography
    id: about
    content:
      title: Biography
      # Choose a user profile to display (a folder name within `content/authors/`)
      username: admin
  - block: features
    content:
      title: Skills
      items:
        - name: Video Editing
          description: Proficient in Adobe Premier & Final Cut Pro
          icon: video
          icon_pack: fab
        - name: Social Media Marketing
          description: Familiar with Twitter, Facebook, Youtube, etc.
          icon: hashtag
          icon_pack: fab
        - name: Data Analysis
          description: Processing and visualization with Python
          icon: python
          icon_pack: fab
  - block: experience
    content:
      title: Experience
      # Date format for experience
      #   Refer to https://wowchemy.com/docs/customization/#date-format
      date_format: Jan 2006
      # Experiences.
      #   Add/remove as many `experience` items below as you like.
      #   Required fields are `title`, `company`, and `date_start`.
      #   Leave `date_end` empty if it's your current employer.
      #   Begin multi-line descriptions with YAML's `|2-` multi-line prefix.
      items:
        - title: Editor
          company: China Global Television Network
          company_url: 'https://www.cgtn.com/'
          company_logo: cgtn
          location: Beijing, China
          date_start: '2021-07-19'
          date_end: '2023-06-30'
          description: |2-
              
              * Managed script-production and post-production for 50+ editions of CGTN's prime time talk show "Dialogue," covering diverse topics like the Russia-Ukraine conflict, China-U.S. relations, Chinese culture, and environment.
              * Conducted topic research, scripted, and facilitated distribution for key documentaries on Taiwan, the Ukraine War and the Middle East.
              * Amplified overseas audience reach by creating and producing 100+ social media posts on platforms such as Twitter, Facebook, Weibo, and WeChat. These posts were cited by 600+ media platforms across 20+ countries, collectively reaching an audience of 270m+.

        - title: Freelance Translator
          company: Pheonix Television
          company_url: 'https://phtv.ifeng.com/english.shtml'
          company_logo: Phoenix
          location: Beijing, China
          date_start: '2019-09-01'
          date_end: '2021-06-30'
          description: |2-
             * Provided precise English-to-Chinese translation for speeches delivered by prominent diplomats and scholars, including the Ambassador of Iran to China, Joerg Wuttke, and the IMF Senior Resident Representative for China.
             * Skillfully translated a range of documentaries, such as "The Great Plague," "Beyond our Earth," and "The Palace & The Press," ensuring accurate and effective communication of complex content.

        - title: Intern
          company: China Institution for Innovation & Development Strategy
          company_url: 'https://www.ciids.cn/gb/en/index.html'
          company_logo: ciids
          location: Beijing, China
          date_start: '2020-10-01'
          date_end: '2020-12-30'
          description: |2-
             * Orchestrated the attendance of 150+ international politicians, academics, and strategists from 20+ countries at the Understanding China Conference 2020. This encompassed guest list preparation, invitations, feedback collection, personal data management, and agenda updates.
             * Translated and published 3 internal publications, converting over 20 speeches by foreign politicians and entrepreneurs from English to Chinese. Included were speeches by figures like former British PM Gordon Brown and Merlin Swire.
             * Coordinated the "Climate Action: China-U.S. Sub-national Cooperation" project. This involved translating project documents, arranging an interview press release with former California Governor Jerry Brown in the Los Angeles Times, curating meeting agendas, recording minutes, and overseeing media coverage tracking.

  - block: portfolio
    id: projects
    content:
      title: Projects
      filters:
        folders:
          - project
      # Default filter index (e.g. 0 corresponds to the first `filter_button` instance below).
      default_button_index: 0
      # Filter toolbar (optional).
      # Add or remove as many filters (`filter_button` instances) as you like.
      # To show all items, set `tag` to "*".
      # To filter by a specific tag, set `tag` to an existing tag name.
      # To remove the toolbar, delete the entire `filter_button` block.
      buttons:
        - name: All
          tag: '*'
        - name: Deep Learning
          tag: Deep Learning
        - name: Other
          tag: Demo
    design:
      # Choose how many columns the section has. Valid values: '1' or '2'.
      columns: '1'
      view: showcase
      # For Showcase view, flip alternate rows?
      flip_alt_rows: false
  - block: markdown
    content:
      title: Gallery
      subtitle: ''
      text: |-
        {{< gallery album="demo" >}}
    design:
      columns: '1'
  - block: collection
    id: featured
    content:
      title: Featured Publications
      filters:
        folders:
          - publication
        featured_only: true
    design:
      columns: '2'
      view: card
  - block: collection
    content:
      title: Recent Publications
      text: |-
        {{% callout note %}}
        Quickly discover relevant content by [filtering publications](./publication/).
        {{% /callout %}}
      filters:
        folders:
          - publication
        exclude_featured: true
    design:
      columns: '2'
      view: citation
  - block: collection
    id: talks
    content:
      title: Recent & Upcoming Talks
      filters:
        folders:
          - event
    design:
      columns: '2'
      view: compact
  - block: tag_cloud
    content:
      title: Popular Topics
    design:
      columns: '2'
  - block: contact
    id: contact
    content:
      title: Contact
      subtitle:
      text: |-
        Feel free to contact me via:.
      # Contact (add or remove contact options as necessary)
      email: qd2177@columbia.edu
      phone: (551)-331-3654
      address:
        street: 419 W115th Street
        city: New York
        region: NY
        postcode: '10025'
        country: United States
        country_code: US
          # Automatically link email and phone or display as text?
      autolink: true
      # Email form provider
      form:
        provider: netlify
        formspree:
          id:
        netlify:
          # Enable CAPTCHA challenge to reduce spam?
          captcha: false
    design:
      columns: '2'
---
