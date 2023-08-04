---
title: "Stor video"
tags: [inspiration]
header:
  video:
    id: 8Uug9_03nR0
    provider: youtube
---

Detta är ett test med så kallad *header video*. Det är en inbäddad video som visas i full bredd högst upp i inlägget. Videospelaren är responsiv.

För att skapa ett sånt här inlägg lägger du in följande i sidans front matter:

```yaml
header:
  video:
    id: 8Uug9_03nR0
    provider: youtube
```

- __*provider*__ är ```youtube``` eller ```vimeo``` (oklart om det finns stöd för fler).
- __*id*__ är videons id. På YouTube hittar du det i URL:en (exempelvis https://www.youtube.com/watch?v=```8Uug9_03nR0```)
---

Om du istället vill infoga en video som vanligt i ett inlägg använder du istället en *include* med samma parametrar.

```liquid
{% raw %}{% include video id="8Uug9_03nR0" provider="youtube" %}{% endraw %}
```

{% include video id="8Uug9_03nR0" provider="youtube" %}

