---
title: "Ducky 3D scan"
tags:
  - 3Dscan
  - laserscanner
edits:
  - 2026-08-27
---

<style>
  .half {
    width: 48%;
    max-width: 600px;
  }

  .third {
    width: 30%;
    max-width: 480px;
  }

</style>

# Ducky 3D scan

## Einstar Rockit 3D-skanner

<img class="third" alt="Einstar Rockit"
src="/assets/images/ducky/einstar-rockit-product-photo.webp">

Einstar Rockit är en kompakt, handhållen 3D-skanner som används för att skapa digitala 3D-modeller av verkliga föremål. När man skannar använder man programvaran **EXStar Hub** från tillverkaren **Shining 3D**. Den finns till Windows och macOS.

Einstar Rockit har både WiFi och batteri, vilket gör att man kan använda den trådlöst utan sladdar. Det går också att ansluta den till datorn via USB, vilket är det vanligaste för liknande 3D-skannrar.

Rockit har både blå linjelaser och infrarött ljus för att kunna skanna allt från små detaljer till större objekt med hög noggrannhet.

Den klarar ofta att skanna mörka och blanka ytor utan att man först behöver behandla med spray som tillfälligt gör ytan ljusare och mattare, vilket annars är vanligt vid 3D-skanning.

Einstar Rockit ska vara bättre än föregående generation på att skanna utan markörer, men kan användas både med och utan markörer. Markörer används vid 3D-skanning för att ge tydliga referenspunkter och förhindar att en skanner tappar spårningen. Markörer innebär dock extra arbete att hantera och det är inte alltid praktiskt möjligt att använda dem. En skanner som klarar mer utan markörer är en tydlig fördel.


## Skanna

![](/assets/images/ducky/einstar-scanning-with-blue-lasers.jpg)

Vi skannar ankan genom att flytta skannern så att den avbildar objektet från alla vinklar runt hela objektet. På datorns skärm visas hela tiden vilka områden som vi har täckt. 

Om delar av objektet är skymda kan man göra flera skanningar och sedan pussla ihop dem efteråt, denna process kallas för *registrering*. Här vänder vi senare ankan upp-och-ner för att skanna undersidan.

En av utmaningarna med 3D-skanning är att skannern måste hålla reda på sin position i förhållande till objektet medan den skannar. Det går att utnyttja föremålets utseende och föremålets form för detta, men om det inte räcker till kan man också tillföra markörer som en skanner enklare kan följa. Einstar Rockit kan använda en valfri kombination av samtliga metoder. 

I det här fallet använder vi slumpvis utplacerade markörer med reflexprickar för att underlätta spårningen. Det är då nödvändigt att objektet och markörerna inte rör sig i förhållande till varandra under hela skanningen.

## Beskära

![](/assets/images/ducky/exstar-hub-scan-data-raw.jpg|320)
![](/assets/images/ducky/exstar-hub-scan-data-crop.jpg|320)

Den råa scanningen innehåller förutom ankan, även delar av omgivningen, underlaget och markörerna. I det här steget markerar vi den data vi vill behålla respektive radera och skär bort allt som vi inte vill ta med. Efter det här steget genomför datorn beräkningar för att skapa ett tätt **punktmoln** av det vi har skannat. 

Det krävs en kraftfull dator med mycket RAM-minne för att hantera all data. Ankan är ett relativt litet objekt och utgjorde inte något problem med 16 GB RAM, men större objekt kräver ofta betydligt kraftfullare dator för att överhuvudtaget kunna processas och det kan ta en lång stund. 

## Punktmoln

![](/assets/images/ducky/exstar-hub-point-cloud-no-color.jpg)

Här ser vi punktmolnet som är resultatet av 3D-skanning. Vi kan bedöma hur mycket av objektet och hur detaljerat som vi lyckats avbilda verkligheten. 

Notera att detaljer som näsborrarna och strukturen på hakremmen är med. Vi kan också se att blanka ytor som propelleraxeln, det svarta på hjälmen och den kromade niten är avbildade. Halsbandet, som både är blankt och har svår struktur, har bara delvis kommit med. Notera också att områden under hakan och inuti hjälmen blir som djupa dalar som skannern inte klarar att nå.

![](/assets/images/ducky/exstar-hub-point-cloud-w-color.jpg)

Här ser vi punktmolnet med färg. Själva 3D-skanningen sker med blå laser eller infrarött ljus och ger ingen färginformation. Einstar Rockit har en inbyggd färgkamera och vit belysning, som den använder för att kunna sätta färg på punktmolnet. 

Vid skanning kan man tänka på att omgivande belysning från lysrör eller solen påverkar färgåtergivningen. På ankan ser vi t.ex. att spetsen på näbben ser gul ut trots att hela näbben egentligen är orange och att den gula färgen på kroppen skiftar med skuggor och varierande ljus.

## Ytmodell (mesh)

![](/assets/images/ducky/exstar-hub-meshing.jpg)

Nästa steg är att binda ihop punkterna i punktmolnet till sammanhängande ytor, som kallas för *mesh* (nät av trianglar). Detta sker automatiskt men man väljer inställningar för filtrering, utjämning och strategi för att laga hål i nätet. Detta steg kräver också ganska mycket av datorn.

Mesh-modellen är det färdiga resultatet från 3D-skanningen. Ytorna är täta. Texturer kan appliceras på ytorna, vilket ger mer detaljerat utseende jämfört med det färglagda punktmolnet. Se som exempel dekalen på ankans hjälm. Om hela modellen är vattentät kan den skickas direkt användas för 3D-utskrift, men ofta finns det hål och områden som behöver fyllas i manuellt.

I 3D-skannerprogramvaran finns det verktyg för att orientera modellen mot XYZ-axlarna. Det finns också mätverktyg om man direkt vill ta ut mått på en modell. 3D-skannern är kalibrerad och alla modeller skannas med verklig skala i millimeter.

## Resultat

![](/assets/images/ducky/ducky-mesh-rotating-no-texture.mp4)

![](/assets/images/ducky/ducky-mesh-rotating-w-texture.mp4)

## Visualisering

![](/assets/images/ducky/side-by-side-ar-model-and-real-ducky.jpg)

Vi har exporterat och konverterat 3D-modellen till USDZ som är ett format som används för *augmented reality*. Med en iPhone eller iPad kan man placera det virtuella förmålet på en yta i det verkliga rummet och betrakta det från olika vinklar. Här har vi placerat den 3D-skannade modellen av ankan bredvid den verkliga ankan. Visst är modellen ganska lik originalet.

### Augmented reality

Testa själv att placera ut ankan i ditt rum med AR QuickLook om du har en iPhone eller en iPad.

<div>
    <a rel="ar" href="/assets/3d/ducky3.usdz">
        <img src="/assets/images/ducky-1024.jpg">
    </a>
</div>
