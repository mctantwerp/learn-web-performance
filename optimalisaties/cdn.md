---
description: Content Delivery Network
---

# CDN

Een **CDN** of voluit **Content Delivery Network** neemt een het probleem van geolocatie en "files" op het internet weg. Om een CDN goed te kunnen begrijpen moeten we eerst begrijpen hoe het internet werkt en hoe request in hun werk gaan zonder dat we gebruik maken van een CDN.

### Zonder CDN

![Voorbeeld van verschillende requests zonder CDN](../.gitbook/assets/image%20%2810%29.png)

Wanneer je als gebruiker bvb een afbeelding van een website wil inladen dan zal zijn requests een hele weg moeten afleggen alvorens het bij de server is. Stel dat er onderweg veel verkeer is \(Ook het internet kent verkeersdrukte en knooppunten\), dan zal de gebruiker hier van hinder ondervinden. Of stel dat de server waar de afbeelding op gelocaliseerd is zich in de VS bevind en de gebruiker zich in Japan bevind? Dan zal de request de hele wereld moeten afreizen alvorens deze bij de server geraakt.

### Met CDN

![Voorbeeld van verschillende request m&#xE9;t CDN](../.gitbook/assets/image%20%2811%29.png)

Wanneer we gebruik maken van een CDN dan zal de content \(bvb: afbeeldingen\) verspreid en gedupliceerd staan over meerdere servers. Wanneer een gebruiker een afbeelding opvraagd dan zal hij naar de dichtsbijzijnde CDN-server \(Of edge server\) gestuurd worden. Als deze server de gevraagde afbeelding heeft dan zal de server die onmiddelijk terugsturen naar de gebruiker. De request is dus minder lang onderweg omdat deze niet de hele wereld moet rondreizen en niet alle drukke knooppunten moet passeren.

Belangrijk om te weten is wel: Wanneer de CDN-server \(of edge server\) de gevraagde afbeelding niet heeft dan zal deze server de afbeelding vragen aan de originele server \(Origin server\). Er wordt dan geen snelheidswinst geboekt. Enkele volgende gebruikers zullen dan profiteren van het feit dat de edge server deze afbeelding al eens heeft ingeladen en cached voor volgende requests.

{% page-ref page="caching.md" %}



