---
title: 'Software ontwerp in C/C++: Project opdracht 2018-19'
accent: "#008eb3"
disableComments: true
---

&laquo;&nbsp;[Terug naar Software ontwerp in C/C++](/teaching/cpp)<br/>

## Project resultaten 2018 - 2019

{{< vimeo 314203871 >}}

## Project opdracht - tweede kans

Dezelfde **minimumvereisten** gelden als hieronder. Werk met een _nieuwe_ Github repository, en vertrek opnieuw vanaf de `gba-sprite-engine`. Geregistreerde tijd bijhouden is niet meer nodig. 

De opdracht is _niet_ vrij te kiezen. Het criteria 'originaliteit' zal beoordeeld worden op de manier waarop je deze vaste opdracht hebt ingekleurd. 

#### Opdracht beschrijving

Ontwerp een **Mario Party kloon**. In dit _bordspel_ gaan spelers op een klassieke manier het bord rond om punten te verzamelen. De structuur van het bord is gelijkaardig aan een Ganzenbord spel. Elke plek waar de speler zijn of haar pion terecht komt, brengt een bepaalde actie met zich mee. In Mario Party wordt er meestal een minigame gespeeld, dat indien gewonnen punten oplevert. Hier is een video van de officiële GBA implementatie:

{{< youtube dvC4hgoNOfE >}}

<br/>
Wat moet minimaal aanwezig zijn?

* Een titelscherm.
* Een bord. De layout maak je zo simpel of complex als je zelf wenst. 
* Een pion die de speler voorstelt. De mogelijkheid om vakjes te verschuiven. 
* Tenminste één (zeer eenvoudig) minigame. De inhoud mag je zelf bepalen. 
* Zichtbaarheid van de score. 

Wat is optioneel?

* Extra spelers in de vorm van AI. 
* Extra minigames. 
* Keuze van de pion.
* Animaties en geluid.

Inleverformaat op dezelfde manier als in de eerste kans. Deadline op vrijdag, 23 augustus 2019, 12u 's middags.

## Project opdracht - eerste kans

Om jullie recent bijgeslepen object-geörienteerde technieken te laten zien gaan jullie een **GBA spel** ontwerpen en ontwikkelen in C++11. De focus van de opdracht ligt niet op correcte low-level IO mapping maar op kritisch denken en testen zoals gezien in [labo 7](/teaching/cpp/labo-7). Uiteraard komen zowel pointers en GBA programming technieken van de vroegere labo's, als C++ class inheritance en abstractie lagen uit de latere labo's aan bod. 

Vertrek vanuit de [gba-sprite-engine](https://github.com/wgroeneveld/gba-sprite-engine/) library die ik gebouwd heb op <i class='fa fa-github'></i> Github door een <i class='fa fa-code-fork'></i> Fork te nemen met de knop rechtsboven. Op die manier bespaar je veel werk met een nieuw GBA project op te zetten en alle IO adressen opnieuw te mappen. Er is een README voorzien voor meer info. De engine gebruikt [Tonc](https://www.coranac.com/tonc/text/toc.htm) achterliggend. 

Wat voor soort spel het moet zijn laat ik volledig aan jullie over. Het spreekt voor zich dat complexiteit (en originaliteit!) mee in rekening gebracht wordt: zie evaluatiecriteria. Inspiratie nodig? 

* [Top 10 Gameboy Advance games in 10 minutes](https://www.youtube.com/watch?v=2-R-F-A48FI)
* [25 Best Gameboy Advance games Ever](http://www.denofgeek.com/us/games/game-boy-advance/256070/25-best-game-boy-advance-games-ever)

Werk in **groepen van 2** of indien oneven 3. 

In het kader van onderzoek naar onderwijs ﻿vragen wij jullie je tijd gespendeerd aan het project bij houden in een bestandje. Dit mag niet veel administratie vragen: enkel in een simpele CSV bijhouden op welke dag jullie hoeveel tijd werk aan het project spendeerden is voldoende. De eenheid is in uren - een halfuur kan bijvoorbeeld met 0.5 uitgedrukt worden. 
Dit is een voorbeeld bestandje:
[https://github.com/wgroeneveld/gba-sprite-engine/blob/master/timespent.csv](https://github.com/wgroeneveld/gba-sprite-engine/blob/master/timespent.csv). 
Wanneer jullie het project in Github overnemen komt deze file automatisch mee. 
Werk dit tijdig bij, dat voorkomt moeten gokken. Dit is individueel dus als jullie samen aan een project werken, maak dan twee files aan!

Bedankt om mee te werken aan een beter onderwijs!

## Minimumvereisten

Lees dit goed na: projecten die niet voldoen aan de volgende vereisten zullen niet geëvalueerd worden. 

1. De code leeft in een repository op Github onder jullie username met de [MIT](https://help.github.com/articles/licensing-a-repository/#disclaimer) license. 
2. Je vertrekt vanuit `gba-sprite-engine` - zie hierboven. Daarbij blijf je binnen GBA `MODE0` en werk je met sprites. C++11 is hiermee ook een vereiste.
3. Indien je je baseert op andere bestaande code doe je aan **bronvermelding**! Plagiaat wordt zeer ernstig bestraft. 
4. Je project moet uiteraard minstens compileren.
5. Je repository `README.md` bevat een kleine functionele beschrijving van jullie spel.
6. Naast de functionele beschrijving upload je ook een schets van je **domein model**, gepaard met verklarende tekst. 
7. Je repository `timespent.csv` bevat jullie **individueel** geregistreerde tijd in uren.  

Het is **niet** de bedoeling om je te baseren op één van de engine demo's en die simpelweg verder uit te werken. Dat biedt onvoldoende uitdaging en originaliteit. 

Omdat als vereiste elk project op Github leeft kunnen jullie elkaar's repository ook raadplegen. Of jullie daar gebruik van willen maken laat ik aan jullie over: onthoud _sharing is caring_ en vergeet de bronvermelding niet. Het is geen race voor het beste waarbij je je code zorgvuldig moet afschermen: iedereen vertrekt vanuit dezelfde basis en iedereen kiest een ander soort spel.

## Evaluatiecriteria

Punten worden op twee keer op `/20` gegeven. Eenmalig een globaal cijfer, eenmalig een genormaliseerd cijfer, rekening houdend met de volgende subcriteria en gewichten:

1. `O.5` Design<br/>
Hoe is je Object-Oriented design en domein model?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: duidelijk herkenbare objecten, terug te vinden in domein model, met gescheiden verantwoordelijkheden. </span>
2. `O.5` Clean Code<br/>
Hoe leesbaar is je code?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: eenvoudig begrijpbare variabelen, methodes, klassen.</span>
3. `0.1` C++ Conventies <br/>
Is je code opgebouwd volgens de aangeleerde C++11 standaarden?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: correct gebruik van header/source files, smart pointers, STL, templates, naamgeving conventies hoofdletters. </span>
4. `0.3` Complexiteit <br/>
Hoe moeilijk heb je het gemaakt?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: gekozen voor een uitdaging in de plaats van een eenvoudige implementatie.</span>
5. `0.3` Originaliteit <br/>
Met welke insteek heb je je idee vorm gegeven?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: een origineel idee uitgewerkt in plaats van een standaard 2D platformer.</span>
6. `0.2` GBA UI <br/>
Hoe uitgebreid is de grafische representatie?<br/>
<span style="color: lightgrey; font-style: italic;">Hoge score: alle UI technieken uitgebreid toegepast: tiles, sprites, scrolling backgrounds, ...</span>

Waarbij beide cijfers herleid worden tot één. <br/>
Bovenstaande criteria zijn herzien op 05/12/2018 en finaal voor academiejaar 2018 - 2019. 

## Inleverformaat

Datum te bepalen, evenals verdedigingsdata.

* Je mailt je github repository URL door, samen met een gecompileerde `.gba` ROM die je zelf getest hebt. 
* De gecompileerde ROM upload je ook naar Toledo.
* Er hangt ook een kleine verdediging aan vast zodat ik kan valideren of je voldoende kennis hebt over de code van je eigen spel. We spelen samen het spel en overlopen de code, waarbij er geantwoord wordt op enkele vragen die invloed uitoefenen op het globaal cijfer. 

## Praktische tips

* Begin bij het begin: werk een concept uit **op papier** en teken dan een ruw model uit. Dit model is onderhevig aan verandering naargelang de ontwikkeling. Vergeet het finale model niet toe te voegen aan de README.
* **Hou het simpel** en werk gradueel iets complexer uit. Wees niet te overmoedig: een zeer goede implementatie scoort hoger dan een slappe complexe.
* Denk voor stukjes met logica eerst aan unit testen. Een test die slaagt helpt je al een heel eind verder. 
* Test je spel tijdig op de mGBA emulator, of in de GBA zelf met een flashcard. 
* Gebruik het voordeel van git: check in op regelmatige tijdstippen, zelfs meerdere keren per dag, wanneer iets werkt. Op die manier bespaar je jezelf een hoop werk als er iets teruggedraaid moet worden. 
* Denk aan concepten die je geleerd hebt in andere programmeervakken, zoals Model-View-Controller (MVC) in "Software ontwerp in Java". [Separation of Concerns](https://en.wikipedia.org/wiki/Separation_of_concerns) is ook in C++ van toepassing. 