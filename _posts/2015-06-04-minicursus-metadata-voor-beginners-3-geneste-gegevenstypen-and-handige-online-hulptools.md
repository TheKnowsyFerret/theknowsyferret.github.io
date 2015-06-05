---
layout: post
title: "Minicursus Metadata voor beginners (3) - Geneste gegevenstypen
&amp; handige online hulptools"
description: "In het derde en laatste deel van deze cursus zal ik ingaan op de ietwat complexere, geneste gegevenstypen. Daarnaast zal ik twee handige online tools die jou kunnen helpen bij het  toevoegen van metadata aan je HTML en het testen ervan."
modified: 2015-06-04 14:41:34 +0200
tags: [cursus, metadata, html, structured data markup helper, structured data tessting tool]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---

<figure>
<img src="/images/test-metadata.jpg" alt="Het testen van je metadata">
<figcaption>Originele foto: <a href="http://bit.ly/1KOESpe">Dave
Bleasdale</a>
</figcaption>
</figure>

In het <a href="http://theknowsyferret.github.io/minicursus-metadata-voor-beginners-2-itemscope-itemtype-en-itemprop/">tweede deel</a> hebben we metadata toegevoegd aan onze webpagina’s. Als uitgangspunt namen we een enkel gegevenstype. 

In het derde en laatste deel van deze minicursus zal ik ingaan op de
ietwat complexere, geneste gegevenstypen. Daarnaast zal ik twee
handige online tools bespreken, die jou kunnen helpen
bij het toevoegen van metadata aan je HTML en het testen ervan.

<h2>Geneste items</h2>
Soms kan het zo zijn dat de eigenschap van een gegevenstype een
gegevenstype op zichzelf is. Ook deze kun je weer bepaalde
eigenschappen meegeven.<br>
Het volgende voorbeeld, overgenomen van
Schema.org zelf, geeft aan dat de webpagina over een film gaat. De naam
van de film is “Avatar”, het genre is science fiction en James Cameron
is de regisseur.

<figure>
<img src="/images/metadata-zonder-nesting.png" alt="Voorbeeld van
broncode met toegevoegde microdata, zonder geneste gegevenstypen.">
</figure>

James Cameron is echter niet alleen regisseur, maar ook een <a
href="https://schema.org/Person">Persoon</a>. Wil je deze informatie
ook verwerken, dan creëer je een genest gegevenstype.

In de broncode doe je dit door direct na de corresponderende
<em>itemprop</em> een nieuwe <em>itemscope</em> en <em>itemtype</em>
toe te voegen. In dit voorbeeld is dat na de <em>itemprop</em>
“director”. Vervolgens kun je de persoonseigenschappen “name” en
“birthDate” toevoegen:

<figure>
<img src="/images/metadata-genest-gegevenstype.png" alt="Voorbeeld van
broncode met een genest gegevenstype.">
</figure>

En heel belangrijk...vergeet niet om dat deel van de broncode dat
betrekking heeft op “Person”, in een apart div element te zetten!


Voegen we nu alles bij elkaar, dan krijgen we de onderstaande code. Het geneste gegevenstype "Person" is te vinden binnen het rood
gemarkeerde div element:

<figure>
<img src="/images/geneste-microdata-volledige-code.png" alt="Broncode
voor een gegevenstype met het geneste gegevenstype Person.">
</figure>


<h2>Google’s Structured Data Markup Helper </h2>
Vind je het implementeren van metadata lastig om zelf te doen? Geen
nood, want de Sturctured Data Markup Helper helpt je hierbij. 

<em>Stap 1: open de Markup Helper</em><br>
Zorg dat je op Google bent ingelogd en surf naar de volgende URL: <a href="https://www.google.com/webmasters/markup-helper/">https://www.google.com/webmasters/markup-helper/</a> 

Dit is wat je ziet:

<figure>
<img src="/images/structured-data-markup-helper.png" alt="Startpagina
van Google's Structured Data Markup Helper">
</figure>

Zoals je kunt zien kun je ook metadata aan e-mails
toevoegen. Aangezien deze minicursus over webpagina’s gaat, kies ik
voor de tab met de naam “Website”.

<em>Stap 2: bepaal welke gegevenstypen je wilt gebruiken</em><br>
Nu is het tijd om aan te geven waar de webpagina over gaat. De tool geeft hiervoor 10 opties:
<ul>
<li>Artikelen</li>
<li>Lokale bedrijven</li>
<li>Restaurants</li>
<li>TV afleveringen met ratings</li>
<li>Boekreviews</li>
<li>Films</li>
<li>Software applicaties</li>
<li>Evenementen</li>
<li>Producten</li>
<li>TV afleveringen</li>
</ul>

Dit lijken weining opties, maar voor de meeste webpagina’s kun je hier
aardig mee uit de voeten. Als voorbeeld voor deze cursus gebruik ik “Artikelen”.<br>

Mocht je nu toch een webpagina hebben dat
over een heel ander onderwerp gaat, dan raadt Google je aan het
bijbehorende gegevenstype op te zoeken op Schema.org en de
bijbehorende instructies op te zoeken voor het implementeren
ervan. Vervolgens kun je Google’s tool (de Structured Data Testing
Tool, later uitgelegd in dit artikel) voor het testen van
gestructureerde data gebruiken om je HTML te testen en aan te passen.

<em>Stap 3: vul de URL of HTML code van de webpagina in</em><br>
Heb je een bestaande webpagina, dan ligt het voor de hand om een URL
in te geven. Is de webpagina nog niet gepubliceerd, dan kun je de HTML
code invoeren. Ik gebruik de URL van een artikel dat ik eerder heb
geschreven.

<figure>
<img src="/images/invullen-markup-tool-artikel-url.png" alt="Selecteer
'Artikelen' en plak de URL of HTML in het daarvoor bestemde veld,
onderaan in de tool.">
</figure>

Zodra je het gegevenstype en de URL hebt ingevoerd, klik je op
"Start tagging”. De tool vraagt je nu om gegevens van de
webpagina te markeren.

<figure>
<img src="/images/tagging-structured-data.jpg"
alt="De tool vraagt je nu om gegevens te markeren."></figure>

<em>Stap 4: selecteer gegevens en identificeer het juiste gegevenstype</em><br>
Nu is het tijd om de eigenschappen die
bij het gegevenstype horen te markeren. Om de juiste eigenschappen te kunnen
vinden, geeft de tool aanwijzingen in het rechter venster.

De enige eigenschap die hier verplicht is, is “Name”: de
titel van het artikel. De rest is optioneel, maar gewenst.
Markeer de titel aan de linkerkant en klik vervolgens op “Name” in het
keuzemenu, dat als een soort tooltip tevoorschijn komt. 

<figure>
<img src="/images/highlighting-name.jpg" alt="Highlight de titel van
het artikel en klik op 'Name' in de tooltip.">
</figure>

De tool voegt de titel nu automatisch toe aan het rechter venster:

<figure>
<img src="/images/tagging-name.png" alt="De Markup Helper tool voegt de
titel direct achter 'Name'.">
</figure>

Ga vervolgens op zoek naar de rest van de aangegeven eigenschappen en doe hetzelfde. Hoe
meer eigenschappen je kunt markeren en labelen, hoe beter.

Helaas is het niet mogelijk om elke eigenschap op deze manier te markeren en toe te voegen. In dat
geval kun je de “Add missing tags” knop gebruiken. Deze staat
onderin het rechter venster. In mijn geval wil ik de URL van de pagina
toevoegen. Ik klik hiervoor eerst op “Add missing tags”. Het
volgende scherm verschijnt:

<figure>
<img src="/images/add-missing-tag.png" alt="Voeg een element in dat je
niet kunt taggen.">
</figure>

In de “Select missing type” sectie selecteer ik vervolgens
"URL". Daarna plak ik de URL van de betreffende webpagina in het veld erachter. Tot slot klik ik op “Save” om de URL op te slaan.

<figure>
<img src="/images/added-url.jpg" alt="Na het selecteren van de optie
'URL' en het invullen van de URL van de webpagina, voegt de tool deze
toe aan het rechter venster, achter URL.">
</figure>

Soms is het niet mogelijk om een eigenschap te markeren,
    omdat deze gewoonweg
niet op je webpagina vermeld staat. In mijn geval is dat bijvoorbeeld
een rating. Dat is niet erg. Je kunt deze gewoon leeg laten. 

Heb je nu alle relevante eigenschappen gemarkeerd, dan kun je de HTML gaan
    bekijken.

<em>Stap 4: Creëer HTML</em><br>
Klik op “<em>Create HTML</em>” linksboven in het scherm. Zodra je
    dit hebt gedaan verandert het rechter venster naar een venster met
	HTML, waarbij de microdata die je zojuist hebt gemarkeerd, is
	toegevoegd aan de broncode. Deze toevoegingen zijn duidelijk
	aangegeven aan de hand van gele highlights:
<figure>
<img src="/images/html-with-microdata.jpg" alt="De microdata is
         toegevoegd aan de HTML broncode en is geel
         gemarkeerd.">
</figure>

<em>Stap 5: Download de microdata of voeg deze toe aan je HTML</em><br>
Als jouw CMS het toelaat om HTML toe te voegen door simpelweg te kopiëren en plakken, dan kun je op “Download” klikken. Hierbij ben je overigens niet verplicht om de volgende opmerking over te nemen: 

<figure>
<img src="/images/opmerking-markup-tool.png" alt="Opmerking van de tool die je niet in je HTML hoeft over te nemen.">
</figure>

Klik je op “Finish” dan krijg je een uitgebreide stap-voor-stap-instructie hoe je je gegenereerde microdata kunt
    toevoegen aan je HTML broncode. 
    
    
<h2>Google's Structured Data Testing Tool</h2>
Om de zojuist toegevoegde microdata te valideren (te checken op
                                                  volledigheid en/of
                                                  fouten), kun je
                                                      gebruik maken
                                                          van de “<a href="https://developers.google.com/structured-data/testing-tool">Structured Data Testing Tool</a>” van Google.<br>
                                                      
                                                      
Aangezien ik zojuist de HTML code heb gedownload, plak ik deze in het linker venster en klik op “Validate.”

<figure>
<img src="/images/structured-data-testing-tool.png" alt="De Structured
         Data Testing Tool">
</figure>

Vervolgens krijg ik in het rechter venster te zien wat goed of fout
    is. In mijn geval is alles goed en zitten er geen fouten in mijn broncode:

<figure>
<img src="/images/results-testing-tool.png" alt="De Structured Data
         Testing Tool geeft aan wat goed of fout is.">
</figure>


<h2>Het einde van deze minicursus Metadata</h2>
Dit is alweer het einde van de minicursus Metadata. In deze minicursus heb ik uitgelegd hoe je op eenvoudige wijze metadata kunt toevoegen aan je webpagina’s. Daarnaast heb ik enkele handige online tools laten zien waarmee je niet alleen metadata kunt toevoegen, maar ook kunt testen op juistheid.<br>
Met deze informatie ben je in staat in korte tijd je webpagina’s te verrijken met verschillende soorten gegevens, waarmee je zoekers helpt bij het zoeken van relevante informatie en waarmee je zoekmachines duidelijk kunt maken waar je webpagina’s over gaan. 

Hebben jullie interesse in meer van dit soort cursussen? Laat het mij dan weten!


