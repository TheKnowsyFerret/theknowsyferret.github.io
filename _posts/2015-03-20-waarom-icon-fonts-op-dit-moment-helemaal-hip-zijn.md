---
layout: post
title: "Waarom icon fonts op dit moment helemaal hip zijn"
description: "Wie rasterafbeeldingen gebruikt om icoontjes op websites
weer te geven, zal bekend zijn met de tekortkomingen van deze
methode. Icon fonts maken korte metten met deze problemen en zijn
daarom erg populair. Maar...ze bieden nog meer voordelen!"
modified: 2015-03-20 14:23:28 +0100
tags: [icon fonts, webdesign]
image:
  feature: 
  credit: 
  creditlink: 
comments: true
share: true
---
<link
href="//maxcdn.bootstrapcdn.com/font-awesome/4.3.0/css/font-awesome.min.css"
rel="stylesheet">
<style>
.text-danger {
 color: rgba(150, 40, 20, 0.8);
}
</style>
<figure>
<img src="/images/icons.jpg" alt="Witte icoontjes op een zwarte achtergrond.">
<figcaption>Foto: <a href="http://bit.ly/1OdF7up">The Open Dept.</a></figcaption>
</figure>




Wie rasterafbeeldingen gebruikt om icoontjes op websites weer te
geven, zal bekend zijn met de tekortkomingen van deze methode.<br>
Zo leidt het gebruik van veel icoontjes tot veel HTTP-verzoeken aan de
browser en kan de bestandsgrootte van een afbeelding erg groot
zijn. In beide gevallen duurt het langer voordat de website geladen
is.<br>
Daarnaast zorgen het inzoomen en het gebruik van hoge resolutieschermen voor vage afbeeldingen.

Icon fonts maken korte metten met deze problemen en zijn daarom erg
populair. Maar...ze bieden nog meer voordelen!

<h2>Wat zijn Icon fonts?</h2>
Icon fonts zijn fonts die volledig uit afbeeldingen bestaan. Voor wie
niet weet waar ik het over heb: denk maar eens aan Webdings, Wingdings
en Dingbats van vroeger.<br>
Op dit moment is er een enorm aanbod aan icon fonts te vinden, die je gratis of tegen betaling kunt downloaden en gebruiken.<br> 
Heb je eenmaal een leuk icon font gevonden, dan kun je deze met behulp
van CSS gemakkelijk op je website weergeven en naar wens aanpassen.

<h2>De voordelen</h2> 
Zoals gezegd bieden icon fonts voordelen boven het gebruik van rasterafbeeldingen. Maar welke zijn dit dan?
<ol>
<li>Icon fonts zijn vector-gebaseerd, waardoor ze resolutie-onafhankelijk zijn. Dit houdt in dat de icoontjes altijd haarscherp zijn.</li>
<li>In tegenstelling tot rasterafbeeldingen, is er bij icon fonts sprake van een enkel bestand en dus maar één HTTP-verzoek.</li>
<li> bestandsgrootte is aanzienlijk kleiner dan bij rasterafbeeldingen, zodat de laadtijd van de website nagenoeg gelijk blijft.</li>
<li>Aangezien een icoon hier in feite een font is, kun je met behulp van CSS eenvoudig de kleur, vorm, transparantie of grootte van een individueel icoon aanpassen.</li>
<li>Ook kun je het icoontje animeren met CSS3 (<i class="fa fa-circle-o-notch fa-spin animated"></i>
).</li>
<li>Net als bij rasterafbeeldingen, kun je icon fonts roteren, schaduw
toevoegen en de opaciteit aanpassen. Ook kun je icoontjes combineren:
<br><br>
<span class="fa-stack fa-lg">
  <i class="fa fa-twitter fa-stack-1x"></i>
  <i class="fa fa-ban fa-stack-2x text-danger"></i>
  </span>
  </li>
</ol>


<h2>Enkele aspecten om rekening mee te houden</h2>
Klinkt allemaal goed, maar toch zijn er een drietal zaken waar je rekening mee moet houden als je icon fonts gaat gebruiken:


Ten eerste moeten browsers van webbezoekers ondersteuning bieden aan de CSS eigenschap “@font-face”, welke voor de weergave van het icon font zorgt.
Dit volgens de website <a
href="http://caniuse.com/#search=%40font-face">caniuse.com</a> niet
altijd het geval.<br>
Zo bieden IE6-8, iOS Safari 3.2-4.1, Android 2.2-3 en Blackberry
Browser 7 slechts gedeeltelijke ondersteuning. Firefox 2-3,
Safari 3.1, Opera Mini 8 en Android Browser 2.1 helemaal geen
ondersteuning.<br>
Wie poblemen met weergave wil voorkomen, doet er daarom goed aan om eerst een check doen
met <a href="http://modernizr.com/">Modernizr</a>. Hiermee kun je testen
of een browser “@font-face” wel of niet ondersteund.<br>
Is dat niet het
geval, dan kun je cruciale icoontjes op de website altijd vervangen
door tekst of een rasterafbeelding van een soortgelijk icoon. Gaat het
om een decoratief icoontje, dan kun je er voor kiezen deze te
verwijderen.<br>
Hoe dit checken, vervangen en verwijderen precies in zijn werk gaat, kun
je lezen in het duidelijke artikel “<a href="http://www.filamentgroup.com/lab/bulletproof_icon_fonts.html"> Bulletproof accessable icon fonts</a>” van de Filament Group. 

Het tweede punt waar je op moet letten, is dat browsers van
webbezoekers ook de
"::before" en "::after" selectoren binnen de content eigenschap voor pseudo elementen ondersteunen.<br>
Vooral  IE8-11 gebruikers ondervinden hiervan nogal wat problemen, vanwege bugs in de browser. Het is dus zaak voor de webontwikkelaar hier goed mee om te gaan. 

Tot slot dien je er rekening mee te houden dat screen readers icon
fonts niet altijd inlezen. Ook komt het voor dat screen readers icon
fonts wel inlezen, maar vervolgens de bijbehorende alfabetische letter
uitspreken en niet de naam van het icoontje. 

Zijn deze tekortkomingen voor jou echter geen probleem of vind je ze te verwaarlozen? Dan zou ik zeggen:
wees hip, doe mee met deze hype en ga lekker aan de slag met icon fonts!



<br><br>
<small>De meest populaire font icons:<br>
<a href="http://fortawesome.github.io/Font-Awesome/">Font Awesome</a><br>
<a href="http://getbootstrap.com/components/#glyphicons">Bootstrap</a><br>
<a
href="http://zurb.com/playground/foundation-icon-fonts-3#allicons">Foundation</a>

<small>Meer informatie over font icons:<br>
Hongkiat.com. <a href="http://www.hongkiat.com/blog/webfont-icons/"> A
guide to: better and sharper UI icons with web fonts</a>. Verkregen
op: 18 maart 2015.<br>
CSS-tricks.com. <a href="https://css-tricks.com/examples/IconFont/">
Icon fonts are awesome</a>. Verkregen op 17 maart 2015.<br>
Codementor.io (2014). <a
href="https://www.codementor.io/design/tutorial/pros-cons-icon-fonts-like-font-awesome-design-tips-developers">
Pros & cons for icon fints like Font Awesome – Design tips for developers</a>.<br>
Occhio.nl (2014). <a
href="http://www.occhio.nl/blog/waarom-iconfonts-cool-zijn/">Iconfonts
zijn cool!</a><br>
</small>

