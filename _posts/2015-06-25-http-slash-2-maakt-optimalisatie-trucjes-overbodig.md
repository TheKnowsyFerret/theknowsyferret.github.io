---
layout: post
title: "HTTP/2 maakt optimalisatie trucjes overbodig"
description: "We trekken continu onze trucendoos open om onze websites
sneller te maken. De komst van HTTP/2 maakt veel van deze trucjes
echter overbodig!"
modified: 2015-06-25 12:22:33 +0200
tags: [http/2, website optimalisatie]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---
<figure>
<img src="/images/netwerk.jpg" alt="Netwerk van draden">
<figcaption>Foto: <a href="http://bit.ly/1IfzKZM">Bruno Girin</a>
</figcaption>
</figure>

Snelle websites scoren hoger op Google en geven een betere gebruikerservaring. Om deze redenen zijn we continu bezig met browser cachen en het optimaliseren van afbeeldingen. Daarnaast maken we gebruik van CDN, voegen we onze scripts en stylesheets samen en ga zo maar door. 

Met de komst van HTTP / 2 zijn veel van deze trucjes echter niet meer
nodig!

<h2>HTTP/2 maakt het internet sneller</h2>
Sinds 1999 communiceren browsers en servers met elkaar via het HTTP/1.1 protocol. Kenmerk van dit protocol is dat voor ieder component op de webpagina een nieuw HTTP-verzoek moet komen om de betreffende informatie te downloaden. 

Gezien de eisen die de huidige internetbezoeker aan het internet stelt, is dit protocol niet langer houdbaar. Daarom werd vorige maand HTTP/2 als officiële opvolger van HTTP/1.1 bekendgemaakt. 

Het doel van dit nieuwe protocol is om het internet sneller te maken,
door efficiënter gebruik te maken van de onderliggende
netwerkverbindingen. Om dit voor elkaar te krijgen, zet HTTP/2 onder
andere de volgende middelen in:<br>

<em>Multiplexing</em><br>
Browsers kunnen met het nieuwe protocol meerdere HTTP-verzoeken tegelijkertijd naar de webserver sturen. Daarnaast kunnen webservers aan meerdere verzoeken tegelijkertijd voldoen. Dit vermindert het aantal actieve connecties aanzienlijk en resulteert in snelheidswinst. 

<em>Server push</em><br>
In plaats van af te wachten tot de browser een bepaald component opvraagt, stuurt de server proactief componenten toe. 

<em>Header compressie</em><br>
Het nieuwe protocol maakt HTTP-headercompressie mogelijk. 

<em>Stream dependencies</em><br> 
De browser kan aan de server doorgeven welke componenten belangrijker zijn dan anderen. Zodoende kan het zelf de volgorde bepalen. 

<em>Verzendt informatie binair in plaats van textueel</em><br>
Binaire informatie is de moedertaal van computers. Alhoewel dit middel niet per se is opgenomen om een sneller internet te bewerkstellingen, leidt het gebruik van binaire informatie wel tot minder fouten.

<em>Werkt goed met beveiligde verbindingen</em><br> 
Via het tls-protocol gaat HTTP/2 efficiënter om met encryptie.


<h2>Wat betekent dit voor jouw website?</h2>
De komst van HTTP/2 maakt vele trucjes om je website sneller te maken,
overbodig. Zo hoef je geen CSS-stylesheets of Javascripts meer samen
te voegen, het aantal plugins te reduceren of Javascript onderaan je
pagina te zetten. Dit betekent dus dat je minder tijd (en geld) hoeft te
spenderen aan website optimalisatie. 

Toch zijn er een aantal taken die je nog steeds kunt (laten)
uitvoeren, omdat ze nog steeds nuttig zijn. Ik denk aan de volgende acties:<br>

<em>Browser caching</em><br>
Alhoewel "Server Push" een groot deel
van de componenten cached, kan expiratie van bepaalde elementen toch
nog handig zijn.

<em>Minificeren</em><br>
Het minificeren leidt nog altijd tot <a href="http://stackoverflow.com/questions/28630108/http2-is-minifying-js-concatenate-js-css-and-using-sprites-no-longer-needed">minder
data</a> en is dus goed om te blijven doen.

<em>Comprimeren</em><br>
Net als minificeren leidt comprimeren tot
minder data.

<em>Het optimaliseren van afbeeldingen</em><br>
Kleinere afbeeldingen
die in het <a
href="http://theknowsyferret.github.io/7-valkuilen-bij-het-gebruik-van-afbeeldingen-op-je-website/">juiste
format</a> zijn gegoten, reduceren de hoeveelheid data.

<em>Gebruik maken van een Content Delivery Network
(CDN)</em><br>
Internationaal gerichte websites kunnen nog steeds
voordeel behalen door hun content dichter bij de gebruiker te plaatsen.


<h2>Browser- en serverondersteuning</h2>
Nu de voordelen van HTTP/2 bekend zijn, rijst de vraag welke browsers
en servers al met het nieuwe protocol werken.

<figure>
<img src="/images/browser-http2.png" alt="Overzicht van browsers die
HTTP/2 ondersteunen.">
<figcaption>Bron: <a href="http://caniuse.com/">www.caniuse.com</a>
</figcaption>
</figure>

Op dit moment maken de huidige versies van 
Chrome, Firefox, Opera, Opera Mobile, Chrome for Adroid en Firefox
for Android volledig gebruik van HTTP/2. IE doet dit gedeeltelijk. De
verwachting is dat EDGE en Safari snel zullen volgen. Grote kans dat je HTTP/2 dus nu al gebruikt!

Voor wat betreft de servers werken bijvoorbeeld Apache, Nginx en IIS al met het
nieuwe protocol.

Wil je een complete lijst inzien en wil je op de hoogte blijven van
alle browsers en servers die
HTTP/2 (gaan) ondersteunen? Dan raad ik je aan het <a
href="https://github.com/http2/http2-spec/wiki/Implementations">implementatieschema</a>
van Mark Nottingham goed in de gaten te houden!

<br>

<small>Bronnen:<br>
Tweakers.com (2015). <a href="http://tweakers.net/nieuws/103109/standaardenorganisatie-publiceert-officieel-http-2-standaard.html">Standaardenorganisatie publiceert officieel
http/2-standaard</a>.<br>
Akamai.com (2015). <a href="https://http2.akamai.com/">HTTP/2 is the future of the Web, and it is already
here</a>!<br>
Zoompf.com (2015). <a
href="https://zoompf.com/blog/2015/01/http2-fast-secure-bedrock-future-seo">HTTP/2:
A Fast, Secure Bedrock for the Future of SEO</a>.<br>
Engadget.com (2015). <a href="http://www.engadget.com/2015/02/24/what-you-need-to-know-about-http-2/">What you need to know about HTTP/2</a>.<br>
</small>
