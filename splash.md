---
title: "ADOPTICUM"
layout: splash
permalink: /splash/
excerpt: "SPECIALISTER PÅ OPTISK MÄTTEKNIK <br/>Vi hjälper er till ökad konkurrenskraft genom tillämpad kamerateknik."

header:
  overlay_color: "#fff"
  overlay_filter: "0.5"
  overlay_image: https://h24-original.s3.amazonaws.com/204790/20568466-QhrEw.jpg
  actions:
    - label: "Senaste inlägg..."
      url: "https://adopticum.github.io/"
  #caption: "Photo credit: Adopticum"

feature_triple:
  - image_path: https://dst15js82dk7j.cloudfront.net/204790/97070969-j6NMI.jpg
    # image_caption: "Image courtesy of [Unsplash](https://unsplash.com/)"
    alt: "Fältarbete"
    title: "Studie & prototyp"
    excerpt: "Adopticum arbetar konkret tillsammans med våra kunder för att hitta lösningar."
    #url: "#test-link"
    #btn_label: "Read More"
    #btn_class: "btn--primary"

  - image_path: https://h24-original.s3.amazonaws.com/204790/20601153-qr1Ht.jpg
    alt: "Topologiskt diagram"
    title: "Skapa lösningar"
    excerpt: "Vi har kompetens att tillämpa tekniken och bygga lösningar som fungerar."

  - image_path: https://dst15js82dk7j.cloudfront.net/204790/99335386-xjICV.jpg
    alt: "3D-skannar person"
    title: "Inspirera & utbilda"
    excerpt: "Vi vill att så många som möjligt ska få se hur roligt och givande teknik kan vara."

feature_a:
  - image_path: https://images.unsplash.com/photo-1587620962725-abab7fe55159
    #- image_path: https://images.unsplash.com/photo-1661956602153-23384936a1d3
    alt: "Källkod på bärbar dator"
    image_caption: "Photo: [Unsplash](https://unsplash.com/)"
    title: "Reserverad plats för innehåll att lyfta"
    excerpt: 'Detta är exempel på innehåll som kan formateras med *Markdown*. Justera bild till vänster med `type="right"`'
    url: "#"
    btn_label: "Läs mer"
    btn_class: "btn--primary"

feature_b:
  - image_path: https://images.unsplash.com/photo-1523348837708-15d4a09cfac2
    alt: "Små plantor i krukor sett uppifrån"
    image_caption: "Photo: [Unsplash](https://unsplash.com/)"
    title: "Reserverad plats för innehåll att lyfta"
    excerpt: 'Detta är exempel på innehåll som kan formateras med *Markdown*. Justera bild till vänster med `type="left"`'
    url: "#"
    btn_label: "Läs mer"
    btn_class: "btn--primary"

feature_c:
  - image_path: https://images.unsplash.com/photo-1568561586426-10f4ce2dafc5
    alt: "Industriell byggnad"
    image_caption: "Photo: [Unsplash](https://unsplash.com/)"
    title: "Reserverad plats för innehåll att lyfta"
    excerpt: 'Detta är exempel på innehåll som kan formateras med *Markdown*. Justera bild till vänster med `type="center"`'
    url: "#"
    btn_label: "Läs mer"
    btn_class: "btn--primary"
---

{% capture notice_quote %}
> Oavsett användningsområde och bransch kan vi hjälpa er med att välja teknisk lösning eller utveckla system. 
> Vi driver projekt tillsammans med behovsägare, produktägare och andra specialister. 
> Målet är att utveckla nya och innovativa lösningar i teknikens framkant. 
> Vi vill med vår kompetens bidra till ökad konkurrenskraft hos företag verksamma i norra Sverige och ge upphov till nya produkter och tjänster.
>
> -- Kenth Johansson, VD
{% endcapture %}

<div class="notice__info">{{ notice_quote | markdownify }}</div>

{% include feature_row id="feature_triple" %}

{% include feature_row id="feature_a" type="right" %}

{% include feature_row id="feature_b" type="left" %}

{% include feature_row id="feature_c" type="center" %}

