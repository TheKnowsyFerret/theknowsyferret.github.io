---
layout: post
title: "Minicursus Metadata voor beginners (2) - itemscope, itemtype
en itemprop"
description: "In dit tweede deel van de Minicursus Metadata gaan we aan de hand van concrete voorbeelden metadata toevoegen aan onze webpagina’s."
modified: 2015-05-28 08:47:01 +0200
tags: [schema.org, cursus, metadata]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---

<figure>
<img src="/images/metadata-invoeren.jpg" alt="Het toevoegen van
metadata aan je broncode">
<figcaption>Foto: <a href="http://bit.ly/1KqOinL">Dennis Skley</a>
</figcaption>
</figure>

In <a
href="http://theknowsyferret.github.io/minicursus-metadata-voor-beginners-deel-1-schema-dot-org/">
deel 1</a> van deze minicursus heb ik de voordelen van metadata behandeld en <a href="https://schema.org">Schema.org</a>
geïntroduceerd. In dit tweede deel van de Minicursus Metadata gaan we
aan de hand van concrete voorbeelden metadata toevoegen aan de
broncode van onze
webpagina’s.


Dit alles doen we met behulp van <a
href="http://en.wikipedia.org/wiki/Microdata_%28HTML%29">microdata</a>:
contextuele informatie waarmee we de browser duidelijk kunnen maken
waar onze webpagina over gaat.

<h2>Itemscope en itemtype</h2>
Stel, je hebt een webpagina waarop de gegevens van een persoon staan
vermeld. Als eerste moeten we de browser laten weten dat de webpagina
over een persoon gaat. Dit doen we door een <strong>itemscope</strong> en een <strong>itemtype</strong>
attribuut aan een <em>div</em> element toe te voegen.


Met <strong>itemscope</strong> laten we de browswer weten dat het hele
stuk binnen het <em>div</em> element over hetzelfde onderwerp gaat.<br>
Het <strong>itemtype</strong> attribuut definieert vervolgens het concrete onderwerp en
doet dit via een hyperlink naar het betreffende onderwerp op
Schema.org.<br>
In ons voorbeeld is dat: <a href="https://schema.org/Person"> “https://schema.org/Person”</a>. 

In de broncode ziet dit er als volgt uit:

<figure>
<img src="/images/itemscope-itemtype.png" alt="Het labelen van je
broncode als het item type Person">
</figure>

<h2>Itemprop: tekst</h2>
Nu de browser weet dat onze webpagina over een persoon gaat, kunnen we
laten weten welke interessante eigenschappen deze “Persoon”
heeft. Denk maar eens aan de naam, de geboortedatum of het adres van
deze persoon.


Om deze eigenschappen te labelen, maken we gebruik van het <strong>itemprop</strong> attribuut.
Een volledige lijst van eigenschappen (properties) voor ‘Persoon” vind je op <a href="https://schema.org/Person"> “https://schema.org/Person”</a> en ziet er zo uit:

<figure>
<img src="/images/schema-org-properties-person.png" alt="De
eigenschappen, expected types en beschrijving van het itemtype Person">
<figcaption>Bron: <a href="https://schema.org/Person">Schema.org</a>
</figcaption>
</figure>

Alle eigenschappen die ons item kan hebben, staan in de eerste kolom. In de derde kolom staat een beschrijving van elke eigenschap. Verwerken we enkele van deze eigenschappen nu in de broncode, dan krijgen we:

<figure>
<img src="/images/itemprop-tekst.png" alt="Het itemprop attribuut
definieert de eigenschappen naam en
functie">
</figure>

In dit voorbeeld hebben we de naam van de persoon en haar functie
gelabeld. De waarde van <strong>itemprop</strong> is in dit geval de tekst
binnen het <em>span</em> element. Dus: “Annelies van der Burg” en "Hoofdredacteur."

<h2>Itemprop: URL’s</h2>
Willen we nu ook nog een afbeelding of een link aan Annelies van der
Burg toevoegen, dan hebben we te maken met URL’s. In dat geval
plaatsen we het <strong>itemprop</strong> attribuut als volgt in de
betreffende HTML elementen:

<figure>
<img src="/images/itemprop-url.png" alt="Het itemprop attribuut
definieert de eigenschappen URL en image">
</figure>

In beide gevallen verwijst <strong>itemprop</strong> nu naar de "src" en "href" attributen
binnen de HTML elementen.


<h2>Itemprop: datum</h2>
Heb je een datum op de webpagina staan, zoals een geboortedatum, dan
raadt Schema.org aan gebruik te maken van het HTML5
<strong>time</strong> element. Hierdoor kun je makkelijk gebruik maken van <a
href="http://nl.wikipedia.org/wiki/ISO_8601">ISO 8601</a>: de
internationale standaard voor het aangeven van een datum, tijd of
tijdsduur. 

Willen we nu bijvoorbeeld de geboortedatum van Annelies invullen, dan ziet dit er als volgt uit:

<figure>
<img src="/images/itemprop-datum.png" alt="Het itemprop attribuut
definieert de eigenschap geboortdatum">
</figure>

Als je tot hier gekomen bent, heb je de basis te pakken. Je bent nu in
staat om de meeste gegevens op je website te labelen. 

<h2>Minicursus Metadata: deel 3</h2>
In het derde en laatste deel van deze cursus zal ik ingaan op geneste items. Hierbij is een eigenschap van bijvoorbeeld het itemtype “Event” een itemtype op zichzelf en dus weer onder te verdelen in een aantal eigenschappen.
