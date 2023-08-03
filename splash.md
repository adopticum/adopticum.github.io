---
title: "Splash Page"
layout: splash
permalink: /splash/

header:
  overlay_color: "#000"
  overlay_filter: "0.5"
  overlay_image: https://h24-original.s3.amazonaws.com/204790/20568466-QhrEw.jpg
  actions:
    - label: "Senaste inlägg..."
      url: "https://adopticum.github.io/"
  caption: "Photo credit: Adopticum"
excerpt: "Bacon ipsum dolor sit amet salami ham hock ham, hamburger corned beef short ribs kielbasa biltong t-bone drumstick tri-tip tail sirloin pork chop."
intro: 
  - excerpt: 'Nullam suscipit et nam, tellus velit pellentesque at malesuada, enim eaque. Quis nulla, netus tempor in diam gravida tincidunt, *proin faucibus* voluptate felis id sollicitudin. Centered with `type="center"`'


feature_row:
  - image_path: https://dst15js82dk7j.cloudfront.net/204790/99335386-xjICV.jpg
    # image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Field work"
    title: "Study & prototype"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    #url: "#test-link"
    #btn_label: "Read More"
    #btn_class: "btn--primary"

  - image_path: https://h24-original.s3.amazonaws.com/204790/20601153-qr1Ht.jpg
    alt: "Topological graph"
    title: "Develop software"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."

  - image_path: https://dst15js82dk7j.cloudfront.net/204790/97070969-j6NMI.jpg
    alt: "3D scanning person"
    title: "Educate & Inspire"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."

feature_1:
  - image_path: https://images.unsplash.com/photo-1523348837708-15d4a09cfac2
    alt: "Small plats in pots from above"
    title: "Placeholder Feature Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_2:
    #- image_path: https://images.unsplash.com/photo-1661956602153-23384936a1d3
    - image_path: https://images.unsplash.com/photo-1587620962725-abab7fe55159
    alt: "Code on laptop computer"
    title: "Placeholder Feature Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"

feature_3:
  - image_path: https://images.unsplash.com/photo-1568561586426-10f4ce2dafc5
    alt: "Industrial building"
    title: "Placeholder Feature Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_1" type="left" %}

{% include feature_row id="feature_2" type="right" %}

{% include feature_row id="feature_3" type="center" %}

---
