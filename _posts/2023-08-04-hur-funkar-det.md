---
title: Hur funkar det
tags:
  - markdown
  - guide
---

### Mål

När grundjobbet är gjort med att sätta upp skelettet för denna hemsida eller blog kommer det att vara mycket enkelt att följa mönster och exempel från befintliga inlägg och sidor. I det skedet räcker det att man kan __skriva text med Markdown och publicera med Git__.


### Teknik

De här sidorna är byggda med följande teknikstapel:

- GitHub Pages
Fri tjänst för att publicera (statiska) hemsidor direkt från versionshanterat repo.
- Jekyll
Omvandlar text med Markdown till hemsidor med HTML+CSS. Jekyll är redan inbyggd i GitHub Pages och körs automatiskt efter varje ändring.
- minimal-mistakes
Ett tema till Jekyll som jag tycker ser bra ut. Dessutom är det bra dokumenterat och man lär sig mycket om Jekyll+GitHub Pages från dok och exempel från detta tema.


### Avancerat

Om man går man djupare och vill jobba med inställningar, mallar, etc stöter man på några ytterligare tekniker som Jekyll är byggd på. Typiskt finns det exempel att kopiera och klistra från. Men bör förstå YAML grundläggande.

- Konfiguration av Jekyll sker med *YAML*, främst i ```_config.yml```.
- Parametrar och metadata kan definieras i filer som *"front matter"* vilket är YAML.
- Enkel skriptning av sidor för t.ex. automatiska listor av inlägg skapas med *Liquid*-syntax.


### Resurser

Här har jag samlat länkar till de exempel och dokumentation som har varit mest givande för att få detta att funka. 

#### minimal-mistakes

Exempelhemsida byggd med minimal-mistakes tema.
https://mmistakes.github.io/minimal-mistakes/

Koden till exempelhemsidan med minimal-mistakes tema. 
https://github.com/mmistakes/minimal-mistakes/tree/master/docs

Repo för själva minimal-mistakes tema.
https://github.com/mmistakes/minimal-mistakes


#### Jekyll
https://jekyllrb.com/docs/

