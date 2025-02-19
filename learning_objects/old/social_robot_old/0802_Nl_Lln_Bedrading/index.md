---
hruid: sr_bouwenrobot2
version: 3
language: nl
title: "Bedrading en monteren"
description: "sr_BouwenRobot"
keywords: ["Sociale Robot", "AI Op School", "STEM", "Computationeel denken", "Grafisch programmeren"]
educational_goals: [
    {source: Source, id: id}, 
    {source: Source2, id: id2}
]
copyright: dwengo
licence: dwengo
content_type: text/markdown
available: true
target_ages: [12, 13, 14]
difficulty: 3
return_value: {
    callback_url: callback-url-example,
    callback_schema: {
        att: test,
        att2: test2
    }
}
content_location: example-location
estimated_time: 20
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen', 
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-technologie-en-technieken'
]
teacher_exclusive: false
---

# Bouwen van de fysieke robot
## Het moederbord
Je zal gebruik maken van de dwenguino en het bijhorende uitbreidingsbord. Bij het snijden van de uitsparingen zal je hier dus ook plaats voor moeten voorzien!  

Let erop dat deze toegankelijk zijn zodat de USB-kabel comfortabel kan verbonden worden.  

## Bedrading en monteren

Vooraleer je de onderdelen bevestigt op het lichaam van de robot, kan je best eerst de bedrading tussen de dwenguino en de andere componenten voorzien. Dit kan noodzakelijk zijn, omdat er soms maar weinig ruimte overblijft om de draden aan te sluiten als je de component bevestigd hebt.

Onderstaande afbeelding toont welke onderdelen aanwezig zijn op de dwenguino en welke actuatoren hier rechtstreeks op kunnen worden aangesloten.

![](embed/Assemblage1.png "dwenguino")

*Op de dwenguino kunnen rechtstreeks twee dc-motoren worden aangesloten. Het contrast van het lcd-scherm kan worden aangepast. Je kan de dwenguino van stroom voorzien via de USB-kabel of een adapter.*

Op de *extension connector* zal je het uitbreidingsbord kunnen aansluiten (zie afbeelding). Dit is speciaal op maat gemaakt voor de sociale robot en je zal er alle andere sensoren en actuatoren kunnen aansluiten.  

![](embed/pcb.png "Uitbreidingsbord")

### Het uitbreidingsbord

Het voordeel van een uitbreidingsbord te gebruiken is dat bij de connectoren vermeld staat voor welke sensoren of actuatoren ze bestemd zijn. 

![](embed/pcb-inkscape.png "Figuur uitbreidingsbord")

**Opgelet**

Wees voorzichtig wanneer je het uitbreidingsbord en de dwenguino aan elkaar koppelt of van elkaar haalt. De pinnen kunnen gemakkelijk buigen als je te veel kracht gebruikt, waardoor het uitbreidingsbord en de dwenguino niet meer goed op elkaar aansluiten.

### Bedrading
Bij het inpluggen van je pinnen, is het belangrijk dat je de juiste zaken met elkaar verbindt. De sensoren en actuatoren hebben bij hun connectoren zaken zoals '+', '-', 'GND' staan en het is ook belangrijk dat je deze met de overeenkomstige pin op het uitbreidingsbord verbindt.

M.b.v. [deze fiches](embed/Leerlingenfiches.pdf "fiches") kan je dit gemakkelijk doen.  

### Monteren
Eens de bedrading in orde is, kan je de elektronica monteren op het lichaam van de robot.  

Als je moeite hebt om bepaalde zaken vast te maken aan het lichaam, kan je ook hiervoor in de fiches kijken. Daar tonen we je dan hoe je met de hulpstukken snel iets kan vastmaken.