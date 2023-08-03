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
  - image_path: https://images.unsplash.com/photo-1661956602153-23384936a1d3
    alt: "placeholder image 1"
    title: "Placeholder 1"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
  - image_path: https://images.unsplash.com/photo-1587620962725-abab7fe55159
    image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "placeholder image 2"
    title: "Placeholder 2"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
  - image_path: /assets/images/unsplash-gallery-image-3-th.jpg
    title: "Placeholder 3"
    excerpt: "This is some sample content that goes here with **Markdown** formatting."
feature_row_l:
  - image_path: https://dst15js82dk7j.cloudfront.net/204790/97070969-j6NMI.jpg
    alt: "placeholder image L"
    title: "Placeholder Image Left Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Left aligned with `type="left"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_r:
  - image_path: https://dst15js82dk7j.cloudfront.net/204790/99335386-xjICV.jpg
    alt: "placeholder image R"
    title: "Placeholder Image Right Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Right aligned with `type="right"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
feature_row_c:
  - image_path: https://h24-original.s3.amazonaws.com/204790/20601153-qr1Ht.jpg
    alt: "placeholder image C"
    title: "Placeholder Image Center Aligned"
    excerpt: 'This is some sample content that goes here with **Markdown** formatting. Centered with `type="center"`'
    url: "#test-link"
    btn_label: "Read More"
    btn_class: "btn--primary"
---

{% include feature_row id="intro" type="center" %}

{% include feature_row %}

{% include feature_row id="feature_row_l" type="left" %}

{% include feature_row id="feature_row_r" type="right" %}

{% include feature_row id="feature_row_c" type="center" %}
---
