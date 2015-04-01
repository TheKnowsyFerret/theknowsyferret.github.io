---
layout: post
title: "Het parallax effect: 5 mythen ontrafeld"
description: "Wie het internet afstruint om meer te weten te komen over deze techniek, merkt al snel dat er zowel positieve als negatieve kanten aan het parallax effect kleven. Echter, niet alles is waar."
modified: 2015-03-31 16:24:15 +0200
tags: [parallax effect, webdesign, usability, user experience]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---
<figure>
<img src="/images/parallaxjs.png" alt="Screenshot van het parallax effect, gemaakt met parallas.js.">
<figcaption>Screenshot: <a href="http://matthew.wagerfield.com/parallax/">Matthew.wagerfield.com</a></figcaption>
</figure>

Steeds vaker kom je websites tegen die het parallax effect toepassen. Het parallax effect is een mooie techniek waarbij de achtergrond langzamer beweegt dan de elementen op de voorgrond. Het doel van deze techniek is het creëren van diepte in een 2-dimensionale omgeving. 

Wie het internet afstruint om meer te weten te komen over deze techniek, merkt al snel dat er zowel positieve als negatieve kanten aan het parallax effect kleven. Echter, niet alles is waar.

In deze blogpost ontrafel ik 5 van de meest hardnekkige mythen rondom het parallax effect. 

<h2>1. Het parallax effect maakt websites slecht vindbaar voor zoekmachines</h2>
De meest hardnekkige uitspraak is wel dat websites met het parallax effect het slecht doen qua SEO. Dit is NIET waar. 

Op <a href="http://moz.com/blog/parallax-scrolling-websites-and-seo-a-collection-of-solutions-and-examples"> moz.com</a> bespreekt SEO-specialist Carla Dawson 3 verschillende technieken, waarmee je websites met het parallax effect wel degelijk goed vindbaar kunt maken. Ook bespreekt ze de voor- en nadelen van elke techniek. 

<em>Techniek 1: one-page websites en jQuery</em><br>
De eerste techniek draait om one-page webontwerpen die het parallax effect gebruiken en maakt gebruik van de “pushState's” functionaliteit in jQuery.<br>
Hiermee verdeel je de pagina in verschillende secties, welke door de SERP’s geïdentificeerd kunnen worden, elk met hun unieke URL en metadata. Resultaat: een enkele pagina wordt meerdere keren geïndexeerd, voor verschillende content. 

<em>Techniek 2: multiple-page websites en SEO architectuur</em><br>
De tweede techniek richt zich op websites waarbij het parallax effect op meerdere pagina’s wordt toegepast. 

Je begint met het optimaliseren van de webarchitectuur en voorziet elke pagina van keywords. Dit geldt niet alleen voor de tekst, maar ook voor de URL-naam, de gebruikte afbeeldingen, enzovoort. 
Vervolgens bouw je iedere pagina op uit drie lagen, die ieder een andere bewegingssnelheid hebben. 

<ul>
<li>Laag 1 - Deze bevat de achtergrondafbeelding en beweegt met 400px/scroll</li>
<li>Laag 2 - Deze laag bevat de content en beweegt met 200px/scroll</li>
<li>Laag 3 - Deze laag bevat de voorgrond en staat stil</li>
</ul>

Verdere optimalisatie kan nog door het toevoegen van metadata aan de footer (via schema.org en een XML sitemap link).

Een voorbeeld van een website die zo is opgebouwd is xDawson.com:

<figure>
<a href="http://www.xdawson.com/"><img src="/images/parallax-xdawson-seo.jpg" alt="Parallax scrolling effect op een website die uit meerdere pagina's bestaat." title="Klik op de afbeelding om het parallax effect in werking te zien."></a>
<figcaption>Screenshot: <a href="http://www.xdawson.com/">xDawson.com</a></figcaption>
</figure>


<em>Techniek 3: Parallax Scrolling on homepage and regular SEO architecture</em><br>
Met de laatste techniek pas je het parallax effect alleen toe op de
homepage. Daarnaast voeg je ook andere pagina’s (URL’s) aan de website
toe die geen gebruik maken van dit effect, maar die wel
SEO-vriendelijk zijn.

<h2>2. Het parallax effect werkt niet op mobiele apparaten. Je moet
hiervoor een aparte website maken</h2>
Een ander veelgehoord nadeel is dat je een aparte site zou moeten maken voor mobiele apparaten, omdat het parallax effect hier niet werkt. Ook dit is NIET waar. 

<em>Het parallax effect werkt wel op mobiele apparaten</em><br>
Ten eerste zijn er door de inspanningen van webontwerpers
(bijvoorbeeld <a href="http://markdalgleish.com/2012/10/mobile-parallax-with-stellar-js/">Mark Dalgliesh</a>) genoeg oplossingen ontwikkeld, waardoor het parallax effect inmiddels ook prima werkt op mobiele apparaten.<br>

Kijk maar eens naar de presentatie van de nieuwe Mac Book van Apple. Alhoewel enige elementen zijn uitgezet, kun je het parallax effect wel degelijk via je mobiele telefoon ervaren:<br>

<figure>
<a href="http://www.apple.com/macbook/"><img src="/images/parallax-apple.jpg" alt="Apple past het parallax effect toe. Het effect is ook te zien op mobiele apparaten." title="Klik op de afbeelding om het parallax effect in werking te zien. Probeer het daarna eens met je mobiele telefoon."></a>
<figcaption>Screenshot: <a href="http://www.apple.com/macbook/">Apple</a></figcaption>
</figure>

Ook de website van <a href="http://matthew.wagerfield.com/parallax">Matthew Wagerfield</a>, laat een zeer indrukwekkend voorbeeld zien van een parallax effect dat goed werkt op mobiele apparaten. Hij gebruikte hiervoor de Javascript library “parallax.js”, welke hij zelf ontwikkelde.<br>

<em>Een aparte website voor mobiele apparaten is niet nodig</em><br>
Daarnaast is het mogelijk om het parallax effect voor mobiele
apparaten <a href="https://ihatetomatoes.net/make-parallax-website-responsive/">uit te schakelen</a> . Wie een pagina met het parallax effect via een mobiel apparaat bezoekt, krijgt dan gewoon een statische webpagina te zien. Het maken van een aparte website voor mobiele apparaten is dus overbodig.<br>
Ga bijvoorbeeld maar eens naar de hoofdpagina van <a href="https://www.spotify.com/us/">Spotify</a> op je pc en bekijk de pagina daarna maar eens op je mobiel:

<figure>
<a href=""><img src="/images/parallax-spotify.jpg" alt="Spotify past het parallax effect toe, maar schakelt deze uit voor mobiel ." title="Klik op de afbeelding om het parallax effect in werking te zien op je desktop en probeer het daarna op je mobiele telefoon."></a>
<figcaption>Screenshot: <a href="https://spotify.com/us">Spotify</a></figcaption>
</figure>


<h2>3. Websites met het parallax effect zijn lastig te tracken met Google Analytics</h2>
Ook dit is niet waar. Websites met het parallax zijn wel degelijk te tracken via Google Analytics, ook als het gaat om een one-pager.

Ten eerste bestaat er de plugin <a href="http://scrolldepth.parsnip.io/">Scroll Depth</a>.  Hiermee kun je bekijken hoe ver een webbezoeker op je website heeft gescrolld: 25%, 50%, 75% of 100%.

Ten tweede kun je gebruik maken van <a href="http://www.publishr.nl/2014/06/analyseren-van-gebruik-van-one-page-websites-in-google-analytics/">virtuele pageviews</a>. Hiermee kun je zien welke klikacties een webbezoeker op jouw website heeft uitgevoerd. Denk bijvoorbeeld aan het aanklikken van buttons, links of afbeeldingen. Ook specifieke acties, zoals het pauzeren van een video zijn te tracken. 

Tot slot kun je gebruik maken van <a href="(http://www.agileand.me/blog/posts/parallax-analytics-tracking">event tracking</a> in combinatie met jQuery en de jQuery waypoints plugin. Natuurlijk kun je, afhankelijk van je doelstelling, event tracking ook combineren met virtual pageviews.<br>
<br>
Voor wie geïnteresseerd is in de voor- en nadelen van virtuele pageviews versus event tracking, raad ik aan de volgende artikelen te lezen: 
<ul>
<li> “<a href="http://searchengineland.com/virtual-pageviews-or-event-tracking-%E2%80%93-which-is-right-for-you-125615">Virtual pageviews or event tracking - which one is right for you</a>”</li>
<li>“<a
href="http://blog.intlock.com/event-tracking-vs-virtual-pageviews/">Event
tracking vs. virtual pageviews</a>”
<li>“<a href="http://www.webseoanalytics.com/blog/google-analytics-event-tracking-vs-virtual-pageviews/">Google Analytics: event racking vs. virtual pageviews</a>”</li></li>
</ul>

<h2>4. Websites met het parallax effect hebben een lange laadtijd</h2>
Het klopt inderdaad dat websites met het parallax effect vaak een lange laadtijd hebben. Echter, ook hier kun je iets aan doen.

Zo kun je minder animaties of lagen gebruiken. Ook hebben een kleiner
formaat afbeeldingen en vereenvoudigde scripts een positief effect op
de laadtijd.

<h2>5. Websites met het parallax effect genieten de voorkeur boven traditionele websites</h2>
Wie op zoek gaat naar de voordelen van websites met het parallax effect, zal er al snel achter komen dat de meeste artikelen beweren dat dit soort websites de gebruikerservaring positief beinvloedt en dat webbezoekers dit soort sites prefereren boven traditionele websites. Niets is echter minder waar.

Voor zijn <a href="http://docs.lib.purdue.edu/cgi/viewcontent.cgi?article=1025&context=cgttheses">afstudeeropracht</a> ontwierp Dede Frederick twee websites voor een fictief hotel. De ene was een traditionele website, de andere bevatte het parallax effect. Vervolgens onderzocht hij voor beide websites de 5 factoren die de gebruikerservaring bepalen: usability, plezier (enjoyment), amusement (fun - verschilt van enjoyment, omdat er ook een fysiologische reactie is), tevredenheid en visuele aantrekkelijkheid. 

Uit het onderzoek kwam naar voren dat de website met het parallax effect in de ogen van de proefpersonen professioneler naar voren kwam en hoger scoorde op de fun-factor. Echter, op de andere factoren scoorden beide websites gelijk.

De conclusie was dan ook dat zowel traditionele websites als websites met het parallax effect even goed scoren als het gaat om gebruikerservaring en er geen voorkeur bestaat voor websites met het parallax effect.

<br>
Ken jij nog meer onwaarheden rondom het parallax effect?
