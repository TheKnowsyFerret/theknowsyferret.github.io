---
layout: post
title: "Minicursus Metadata voor beginners (1) - Schema.org: een introductie"
description: "In dit eerste deel van de minicursus Metadata beschrijf ik de voordelen van het gebruik van metadata en introduceer ik Schema.org."
modified: 2015-05-21 11:14:59 +0200
tags: [schema.org, cursus, metadata]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---

<figure>
<img
src="/images/schema-org.png" alt="Het logo van Schema.org">
</figure>

Met metadata kun je gegevens aan je webpagina’s toevoegen, waarmee je
de informatie op die webpagina beschrijft. Zo kun je de naam van de
auteur toevoegen, de publicatiedatum of het onderwerp waar de
webpagina over gaat.

Maar waarom zou je eigenlijk metadata willen gebruiken? Wat zijn de voordelen?
En hoe pas je het toe? 

In dit eerste deel van de 3-delige minicursus Metadata beschrijf ik de
voordelen van het gebruik van metadata en introduceer ik <a
href="http://schema.org/">Schema.org</a>: één van de meest gebruikte
standaarden om metadata toe te voegen aan webpagina’s.


<h2>De voordelen van metadata</h2>

Een woord kan verschillende betekenissen hebben. Neem bijvoorbeeld het
woord “Avatar”. Dit kan naar de film verwijzen, een term uit het
Hindoeïsme of naar een zelf gekozen profielafbeelding voor een website
of videospel.


Door metadata toe te voegen aan je broncode, "begrijpen" zoekmachines
om welke  betekenis het gaat. Deze kennis helpt hen vervolgens bij het
opsporen en weergeven van informatie die naadloos aansluit op de
zoektermen en de intentie van zoekers. Zoekers vinden op deze manier
dus sneller de informatie waar zij naar op zoek zijn.


Kortom, je kunt stellen dat het toevoegen van metadata aan je
webpagina’s de volgende voordelen heeft:<br>

<ul>
<li>Je helpt zoekers bij het vinden van wat zij zoeken</li>
<li>Het maakt het web voor iedereen nuttiger</li>
<li>Het verhoogt de effectiviteit van zoekmachines</li>
<li>Het verhoogt de click-through-rate</li>
</ul>

Daarnaast is er nog een voordeel:

<ul>
<li>Het voegt “rich snippets” toe aan de zoekresultaten</li>
</ul>


Standaard zoekresultaten laten de titel, URL en omschrijving van een
webpagina zien. Met metadata kun je het zoekresultaat verrijken met
toegevoegde informatie, zoals een kruimelpad, rating of
afbeelding. Dit noemen we een <em>rich snippet</em>. In Google kan dit
er voor een recept als volgt uit zien:<br>

<figure>
<img
src="/images/rich-snippet-chocolate-brownies.jpg" alt="Een rich
snippet van het recept van en chocolade brownie, zoals getoond door
Google">
<figcaption> Deze <em>rich snippet</em> laat een rating, de bereidingstijd en het
aantal calorieën zien </figcaption>
</figure>

<h2>Wat is Schema.org?</h2>
Voor het toevoegen van metadata kun je kiezen uit verschillende
standaarden. Een van de meest gebruikte is <a
href="http://schema.org/">Schema.org</a>.<br>
Schema.org bestaat sinds 2011 en is een gezamenlijk project van de
zoekmachines Google, Bing, Yahoo! en het Russische Yandex.


Het doel van het project is om tot een gedeelde standaard te komen waarmee je data kunt structureren. Door specifieke “tags” (microdata) aan HTML codes toe te voegen, maak je een zoekmachine duidelijk waar de webpagina over gaat. 

<h2>Waar moet je op letten bij het gebruiken van schema.org?</h2>
Voordat je gebruik maakt van Schema.org, zijn er een zestal zaken die je in je achterhoofd moet houden: 

<em>1. Hoe meer je beschrijft, hoe beter</em><br>
Hoe meer data je beschrijft hoe beter de zoekmachine begrijpt wat de inhoud van je webpagina is en hoe beter je zoekers kunt helpen bij het vinden van relevante informatie. 


<em>2. Beschrijf geen verborgen content</em><br>
Voeg alleen metadata toe aan content dat zichtbaar is voor de lezer. Dus niet voor informatie dat verborgen zit in div’s of andere verborgen elementen. 

<em>3. “Verwachte typen” versus tekst</em><br>
Soms is de eigenschap van een type (d.w.z. het item dat je beschrijft), een type op zichzelf, die je ook weer kunt beschrijven door het toevoegen van eigenschappen. Dit hoef je echter niet te doen. Voel je vrij om hier gewoon tekst te gebruiken of een URL.<br>
Ook is het mogelijk om voor een verwacht type een kind-element van dat type te gebruiken. Als voorbeeld noemt Schema.org get type “Place”. In dat geval is het ook prima om het specifiekere "LocalBusiness" te gebruiken. 

<em>4. Het gebruik van de URL eigenschap</em><br>
Een webpagina kan over een enkel onderwerp gaan of over een collectie van onderwerpen. Neem bijvoorbeeld een webpagina dat de medewerkers van een organisatie laat zien.<br>
Deze kan een specifiek persoon beschrijven of de alle medewerkers. In dat laatste geval zul je voor iedere medewerker metadata moeten toevoegen. Bovendien moet je voor elke medewerker de URL-eigenschap toevoegen aan de link naar zijn of haar profiel. 

<em>5. De metadata moet een 1-op-1 relatie hebben met de content</em><br>
Een inkoppertje, maar de metadata aansluiten op het onderwerp waar de pagina over gaat. Gaat je pagina over treinen, dan mag je dus geen metadata toevoegen over auto’s. 
Doe je dit wel, dan zet je zoekers op het verkeerde spoor. Dit kan je op termijn klanten of bezoekers kosten. 

<em>6. Rich Snippets zijn beperkt tot een aantal typen</em><br>
Niet voor alle onderwerpen laat Google “rich snippets” zien. Op dit moment geldt de ondersteuning alleen voor de volgende items:
<ul>
<li><a href="https://developers.google.com/structured-data/rich-snippets/products ">Products</a></li>
<li><a href="https://developers.google.com/structured-data/rich-snippets/products">Recipes</a></li>
<li><a href="https://developers.google.com/structured-data/rich-snippets/reviews">Reviews</a></li>
<li><a href="https://developers.google.com/structured-data/rich-snippets/reviews">Events</a></li>
<li><a href="https://developers.google.com/structured-data/rich-snippets/sw-app">SoftwareApplications</a></li>
<li><a href="https://developers.google.com/structured-data/rich-snippets/videos">Videos</a></li> 
<li><a href="https://developers.google.com/structured-data/rich-snippets/articles">Articles</a></li>
</ul>

<br>

<h2>Minicursus Metadata: deel 2</h2>
In deel 2 van deze minicursus leer je de basisbegrippen van Schema.org kennen en gaan we metadata toevoegen aan de hand van concrete voorbeelden!

<br><br>
<small>Bronnen:<br>
Projectorganika.com (2013). <a
href="http://projectorganika.com/search-engine-optimization/the-benefits-of-using-schema-org/">The
benefits of using Schema.org</a>.<br>
Internetmarketingninjas.com (2013). <a
href="http://www.internetmarketingninjas.com/blog/search-engine-optimization/schema-org-guide-beginners-cheatsheet/">Schema.org
guide for beginners + Schema cheatsheet</a>.<br>
</small>
