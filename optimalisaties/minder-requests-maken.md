# Minder requests maken

Dit is een techniek die vroeger veel werd gebruikt. Vandaag is deze iets minder populair.

Stel dat je een pagina hebt waar je afbeeldingen van verschillende emoji's wil tonen.

Dan zo je dat op deze manieren kunnen doen:

### Standaard manier \(Niet geoptimaliseerd\)

![Afbeelding 1](../.gitbook/assets/screenshot-18-09-2021at-14.02.47-2x.png)

![Afbeelding 2](../.gitbook/assets/screenshot-18-09-2021at-14.02.43-2x.png)

![Afbeelding 3](../.gitbook/assets/screenshot-18-09-2021at-14.02.37-2x.png)

```text
<div style="background: url('afbeelding_1.png')"></div>
<div style="background: url('afbeelding_2.png')"></div>
<div style="background: url('afbeelding_3.png')"></div>
...
```

### Geoptimaliseerde manier

Met de bovenstaande manier zouden er 3 afbeeldingen apart moeten worden ingeladen. Stel dat je deze 3 afbeeldingen combineert in één afbeelding:

![Gecombineerde afbeelding](../.gitbook/assets/image%20%285%29.png)

```text
<div style="background: url('gecombineerde_afbeelding.png') 10px 10px"></div>
<div style="background: url('afbeelding_2.png') 20px 20px"></div>
<div style="background: url('afbeelding_3.png') 40px 60px"></div>
...
```

Door handig gebruik te maken van de **offset** bij de background property kunnen we het gedeelde dat getoond wordt van de gecombineerde afbeelding manipuleren.

Meer info over de background position vind je [hier](https://developer.mozilla.org/en-US/docs/Web/CSS/background-position)

Dit wordt niet gebruikt voor échte afbeeldingen op je website maar wel voor bvb: icons.



{% page-ref page="images.md" %}



