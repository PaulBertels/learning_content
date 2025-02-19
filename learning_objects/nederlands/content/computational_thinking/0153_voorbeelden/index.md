---
hruid: ct_voorbeelden3
version: 3
language: nl
title: "Bebras en CD"
description: "Bebras en CD"
keywords: [""]
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
estimated_time: 1
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen'
]
teacher_exclusive: true
---
# Basisconcepten computationeel denken in de Bebras-wedstrijd

Het hoofddoel van de Bebras-wedstrijd is om de deelnemers warm te maken voor de informatica. Tijdens de wedstrijd pakken de deelnemers verschillende problemen aan die kunnen gelinkt worden aan concepten uit de informaticawetenschappen. Hierbij wordt dus ook het computationeel en probleemoplossend denken van de deelnemers getest.

> Voor meer uitleg over de internationale Bebras-wedstrijd zie https://www.bebras.be/nl/home

Hieronder vind je een aantal vragen uit de Bebras-wedstrijd met daarbij telkens een beschrijving van welke basisconcepten van computationeel denken je gebruikt om *tot de oplossing te komen van het gestelde probleem*.<br>

De gebruikerslicentie van de Bebras-opgaven is CC BY-NC-SA (Creative Commons Attribution-NonCommercial-ShareAlike 3.0 of later).

## Voorbeeld 1:  Decompositie en abstractie
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Pär Söderhjelm, SE, Artem Iglikov, KZ, Jan Berki, CZ<br>
Afbeeldingen: Maiko Shimabuku, JP

#### Groter en kleiner (Bebras 2014-SE-04)

De jonge bevers Anna, Britt, Charlotte, Demi en Emma - allemaal met een verschillende lengte - willen met jou een spelletje spelen. Ze plaatsen zich in een rij, de ene achter de andere, terwijl ze allemaal in dezelfde richting kijken, in een volgorde die ze zelf hebben gekozen. Elke bever telt dan hoeveel bevers vóór en achter haar groter zijn. Dit zijn de resultaten:

|**Naam**|**Aantal grotere bevers ervoor**|**Aantal grotere bevers erachter**|
|---------------|------------------------|----------------------------|
|Anna|1|2|
|Britt|3|1|
|Charlotte|1|0|
|Demi|0|0|
|Emma|2|0|


*In welke volgorde staan de bevers opgesteld?*

##### Oplossing

Er zijn 5 bevers. <br>
Uit de tabel kan je afleiden dat Demi de grootste is want geen enkel bever ervoor of erachter is groter. Daarna volgt Charlotte met slechts één bever die groter is (nl. Demi), dan Emma, en dan Anna en tot slot Britt. Britt is de kleinste bever want alle vier de andere bevers zijn groter.

![bebrasdecompositiestap1](embed/bebrasdecompositiestap1.png)

Redeneer nu op de volgende manier:<br>
- Omdat iedereen kleiner is dan Demi, is Demi groter dan Charlotte, en moet het Demi zijn die voor Charlotte in de rij staat.   
    - Demi - Charlotte
- Er zijn twee bevers groter dan Emma en die staan voor Emma. Die twee bevers zijn Demi en Charlotte  
    - Demi - Charlotte - Emma
- Omdat slechts één grotere bever voor Anna staat, moet dat Demi zijn. Dus Anna komt na Demi en voor Charlotte en Emma. 
    - Demi - Anna - Charlotte - Emma
- Britt heeft drie grotere bevers voor zich staan, dus staat Britt na Charlotte in de rij. 
    - Demi - Anna - Charlotte - Britt - Emma

![Groter en kleiner](embed/bebrasdecompositieabstractieoplossing.png "Bebras Groter en kleiner oplossing")

##### Bespreking

Dit is een mooi voorbeeld van **decompositie**. In een eerste stap bepaal je voor elke bever hoeveel bevers kleiner zijn dan die bever en dus eigenlijk wat de rangschikking in grootte van de bevers is. Daarna gebruik je deze informatie in een tweede stap om de volgorde van de bevers in de rij te bepalen. 

Bij de oplossing pak je de deelproblemen een voor een aan. Op die manier bekom je telkens tussenresultaten die je dan gebruikt om een volgend deelprobleem op te lossen.

In de eerste stap maak je bovendien een **abstractie** van het verschil tussen ‘ervoor’ en ‘erachter’. Je bent enkel geïnteresseerd in het aantal bevers die groter zijn dan een bepaalde bever, niet of die ervoor of erachter staan.


## Voorbeeld 2:  Algoritme toepassen
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Mathias Hiron, FR<br>
Afbeeldingen: onbekend

#### Naar beneden (Bebras 2012-FR-10)
Mevrouw Bever heeft een robot geplaatst bovenaan een doolhof. De robot daalt het doolhof af van het ene platform naar het andere eronder, totdat hij één van de vakken bereikt helemaal onderaan. Hiebij verplaatst hij zich altijd op dezelfde manier: hij verplaatst zich eerst naar rechts, en telkens wanneer hij een platform naar beneden valt, vertrekt hij opnieuw in de omgekeerde richting.

De linker afbeelding hieronder toont het traject dat de robot zal volgen in het doolhof nr. 1.

![Naar beneden](embed/bebrasalgoritme.png "Bebras algoritme")

*Als mevrouw Bever haar robot helemaal links plaatst in doolhof nr. 2, in welk vak zal de robot dan uiteindelijk vallen?*

##### Oplossing

![Naar beneden](embed/bebrasalgoritmeoplossing.png "Bebras Naar beneden oplossing")

Je vindt de oplossing door het **algoritme** uit te voeren dat is opgegeven.

##### Bespreking

De robot verplaatst zich volgens een gegeven **algoritme**. Dat algoritme moet je begrijpen en toepassen op het tweede doolhof. 

Het algoritme kan als volgt beschreven worden: 

<div class="alert alert-box alert-secondary"><p style="  font-family: 'Courier New', monospace; font-size:12px;">
Herhaal de volgende vier lijnen, zolang je niet beneden bent aangekomen:<br>
&nbsp;&nbsp;&nbsp;&nbsp;Ga verder in de huidige richting, en daarna<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Val naar beneden tot aan het eerstvolgende platform, en<br>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;Keer de huidige richting om
</p>
</div>

Er zijn verschillende manieren om algoritmisch denken in een computationeel denkproces toe te passen. In dit voorbeeld komt algoritmisch denken voor in zijn eenvoudigste vorm is. In de andere voorbeelden maak je kennis met andere vormen van algoritmisch denken.

Mogelijke toepassingen zijn:
- een opgegeven algoritme kunnen toepassen (voorbeeld 2, voorbeeld 4);
- zelf een algoritme bedenken om op een efficiënte manier tot een oplossing te komen (voorbeeld 5).

Een tussenweg waarvan er hier (nog) geen voorbeeld is:  
- een (algemeen) gekend algoritme toepassen om een probleem op te lossen.<br>
Bij deze tussenweg is een vorm van patroonherkenning nodig. Voorbeelden ervan zijn: weten hoe je geld moet teruggeven om zo weinig mogelijk briefjes en munten te gebruiken, een lineaire
vergelijking met één variabele kunnen oplossen ...

## Voorbeeld 3:  Patroon herkennen
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Opráné Vecsei Éva, HU, Zsuzsa Pluhár, HU, Sébastien Combéfis, BE<br>
Afbeeldingen: onbekend

#### IJsjesmachine (Bebras 2013-HU-01)

Een ijsmachine produceert gekleurde bollen op een bijzondere systematische manier. Voor elk hoorntje worden er vier bollen geschept. Hieronder zie je hoe de laatste drie ijsjes eruit zagen die door de machine werden gemaakt:

![IJsjesmachine](embed/bebraspatroon.png "Bebras patroonherkenning")

*Hoe ziet het volgende ijsje eruit dat door de machine wordt gemaakt?*

##### Oplossing

![IJsjesmachine](embed/bebraspatroonoplossing.png "Bebras IJsjesmachine oplossing")

##### Bespreking
In deze opgave wordt er expliciet gevraagd om een **patroon** te herkennen en te extrapoleren. Deze opgave is bedoeld voor heel jonge kinderen en is dus voor iedereen gemakkelijk te begrijpen.

De ijsmachine produceert bollen in vier verschillende kleuren en bovendien in een vaste volgorde die zich steeds herhaalt. Na vier bollen wordt een kleur dus herhaald. Dus de onderste bol van een ijsje heeft altijd dezelfde kleur als de bovenste bol van het vorige ijsje.

De kleuren van de bollen bij de laatste drie ijsjes waren de volgende:<br>
groen - rood - paars - blauw - blauw - groen - rood - paars - paars - blauw - groen - rood<br>
Dus de volgorde 'groen - rood - paars - blauw' wordt steeds herhaald en loopt door van het ene ijsje naar het andere. 

Het volgende ijsje moet dus eerst een rode bol krijgen en daarna 'paars - blauw - groen'.


## Voorbeeld 4:  Algoritme toepassen en patroon herkennen
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Kris Coolsaet, BE<br>
Afbeeldingen: Kris Coolsaet, BE
 
#### Kaarten omdraaien (Bebras 2018-BE-01a)
We spelen het volgende 'spelletje'. Voor je ligt een rij kaarten. Een kaart ligt ofwel met de prent naar boven of met de prent naar onder.

Één stap in het 'spel' gebeurt op de volgende manier:<br>
Je bekijkt de kaarten van rechts naar links.<br>
Als de huidige kaart met de prent naar beneden ligt, dan draai je de kaart met de prent naar boven en je stopt.<br>
Als de huidige kaart met de prent naar boven ligt, dan draai je ze met de prent naar onder en je gaat verder met de kaart links ervan.<br>
Ben je alle kaarten gepasseerd, dan stop je.

De afbeelding hieronder toont het effect van opeenvolgende stappen: je draait eerst de kaart helemaal rechts om, dan de kaart links ervan en dan de kaart links daarvan. En dan moet je stoppen, want de derde kaart ligt nu met de prent naar boven.

![Kaarten omdraaien](embed/bebrasalgoritmepatroon.png "Bebras algoritme en patroonherkenning")

Het spel start met 32 kaarten met alle prenten naar beneden:

![Kaarten omdraaien](embed/bebrasalgoritmepatroonopgave.png "Bebras algoritme en patroonherkenning")

*Hoeveel kaarten liggen met de prent **naar boven** nadat je precies 32 stappen in het spel hebt gedaan? (Antwoord met een getal.)*

##### Oplossing

![Kaarten omdraaien](embed/bebrasalgoritmepatroonoplossing.png "Bebras Kaarten omdraaien oplossing")

Merk op dat na 1 stap, na 2, 4, 8 stappen er telkens 1 kaart met de prent naar boven ligt. Dat zijn stappen 2<sup>0</sup>, 2<sup>1</sup>, 2<sup>2</sup>, 2<sup>3</sup>, alle machten van 2. 32 is ook een macht van 2. Na 32 stappen ligt er 1 kaart met de prent naar boven. 

##### Bespreking

Merk op dat je hier opnieuw een algoritme uitvoert en niet zelf bedenkt, zoals in voorbeeld 2.
Behalve het feit dat je hier een **algoritme** moet uitvoeren, is hier ook sprake van **patroonherkenning**. Tijdens het uitvoeren van het algoritme moet je merken dat er precies één kaart met de prent naar boven ligt na 1 stap, na 2 stappen, na 4 stappen, en dan telkens na het dubbel aantal stappen als de keer ervoor. Het aantal stappen is dus steeds een macht van 2. 32 is 2 tot de vijfde, dus ook dan ligt er één kaart met de prent naar boven. 

Binnenin een computer worden getallen voorgesteld in zogenaamde binaire notatie: een getal wordt 'geschreven' met enkel enen en nullen (bits genoemd).<br>
Bv. 1 wordt voorgesteld als 0...00001, 2 als 0...00010, 3 als 0...00011, 4 als 0...00100, 5 als 0...00101, 6 als 0...00110, enz. (Moderne computers gebruiken vaak 32 bits om een getal voor te stellen.)<br>
Herken je deze patronen? Wanneer je voor bit 0 een kaart met de prent naar beneden legt, en voor bit 1 met de prent naar boven, dan krijg je dezelfde patronen als bij de eerste 6 stappen van ons spel. Als je weet dat de binaire voorstelling van 32 niets anders dan 0...01000000 is, dan zie je dat er na 32 stappen precies één kaart met de prent naar boven ligt.<br>
Wat we in deze puzzel een 'stap' noemen, is wat er door de elektronica van een computer gebruikt wordt om een binair getal met 1 te verhogen.


## Voorbeeld 5:  Algoritme bedenken
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Yukio Idosaka, JP, Yasushi Kuno, JP, Elena Sutkute, LT, Juha Vartiainen, FI, Barbara Müllner, AT<br>
Afbeeldingen: Maiko Shimabuku, JP, Javier Bilbao, ES

#### Kortste route (Bebras 2013-JP-10)

De kleine bever speelt graag in het park. Zijn huis (H) en het park (P) zijn met elkaar verbonden door bruggen, gemaakt van boomstammen van dezelfde lengte, zoals je ziet op de kaart hieronder:

![Kortste route](embed/bebrasalgoritmebedenken.png "Bebras algoritme bedenken")

Er zijn echter enkele plaatsen op de kaart, aangeduid met een rode X, waar hij niet voorbij kan.

*Hoeveel verschillende routes van het huis naar het park kan hij volgen met dezelfde minimale lengte?*

##### Oplossing

ER zijn 18 routes met dezelfde minimale lengte (nl. 9 verplaatsingen, 6 naar rechts en 3 naar boven).

![Kortste route](embed/bebrasalgoritmebedenkenoplossing.png "Bebras Korste route oplossing")

Het aantal mogelijke routes tot aan een bepaald kruispunt is de som van het aantal routes dat van links komt en het aantal dat van beneden komt. (Je mag niet van rechts of van boven komen, want dan moet je ooit terugkeren en dan is het pad niet van minimale lengte.)<br>
Daarom noteer je vanaf links onderaan bij elk kruispunt de aantallen en verplaats je je stap voor stap naar rechts en naar boven. Het getal dat je dan rechtsboven opschrijft, is het uiteindelijke antwoord.

##### Bespreking

De oplossing bestaat uit twee denkstappen: 
- een eerste stap bestaat erin zich te realiseren dat je in een kortste route noodgedwongen nooit naar links of naar beneden beweegt;
- in een tweede stap hoef je dus enkel dergelijke routes te bekijken.

In tegenstelling tot voorbeelden 2 en 4, moet je hier wel zelf een **algoritme** opstellen om tot de oplossing te komen: je moet een systematische manier bedenken om tot die oplossing te komen. <br>
De *brute benadering*, nl. alle mogelijkheden uitproberen en hopen dat je er geen vergeten bent, werkt niet; er is echt nood aan het bedenken van een systematische manier om dit probleem op te lossen (m.a.w. een algoritme).<br>
Bij dit voorbeeld: van linksonder naar rechtsboven werken en telkens bij de boomstammen opschrijven hoeveel wegen ernaartoe leiden.

Merk op dat je hier wel algoritmisch denken nodig hebt, maar niet hoeft te programmeren!

De techniek die je gebruikt om deze opgave op te lossen, heet *dynamisch programmeren*: je verdeelt je probleem in kleinere deelproblemen die je gemakkelijk kan oplossen. In dit geval is het deelprobleem 'hoeveel routes zijn er naar het kruispunt waar we net mee bezig zijn?' Dat aantal routes hangt af van het aantal routes naar het kruispunt waar je net van komt. Je begint daarom links onderaan en je gaat stap voor stap naar rechts en naar boven, en je schrijft bij elk kruispunt de aantallen op tot je rechtsboven aankomt.<br>
*Misschien had je al ervaring met dit soort problemen en herkende je dat dynamisch te programmeren hier misschien snel tot de oplossing zou kunnen leiden.*


## Voorbeeld 6:  Abstractie maken
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Zoltán Molnár, HU, Zsuzsa Pluhár, HU<br>
Afbeeldingen: Ivo Blöchliger, CH

#### Stormbestendig netwerk (Bebras 2014-HU-02) 

De GSM-maatschappij Bever Telecom wil GSM-masten plaatsen op Windeneiland.<br>
Het dekkingsgebied van een mast is een cirkel die errond is gecentreerd. Twee masten heten verbonden met elkaar als hun dekkingsgebieden overlappen. Twee masten kunnen met elkaar communiceren als er een rij tussenliggende masten bestaat zodat elke mast met elke volgende is verbonden.<br>
Door de sterke wind op het eiland gebeurt het af en toe dat een mast breekt. Als er ergens één mast niet meer functioneert, willen we toch nog dat elke twee van de overblijvende torens met elkaar kunnen blijven communiceren.

*Welke van de opstellingen hieronder moeten we hiervoor gebruiken?*

![Stormbestendig netwerk](embed/bebrasabstractie.png "Bebras Abstractie maken")

##### Oplossing

Het juiste antwoord is B. 

![Stormbestendig netwerk](embed/bebrasabstractieoplossing.png "Bebras Stormbestendig netwerk oplossing")

##### Bespreking

In de afgebeelde opstellingen worden masten voorgesteld door punten en dekkingsgebieden door cirkels. Dit is een eerste **abstractie** die je correct moet interpreteren.

Om tot een oplossing te komen, voer je een **bijkomende abstractie** in door de overlappende cirkels te vervangen door een boog in een graaf: je verbindt twee masten met elkaar wanneer de overeenkomstige cirkels overlappen, en je verwijdert de cirkels. Dit is een cruciaal deel van het oplossingsproces.

Abstractie kan dus op twee verschillende manieren voorkomen in computationeel denken:
- een gegeven abstractie correct kunnen interpreteren;
- zelf tot een abstractie komen om een probleem gemakkelijker op te lossen.


## Voorbeeld 7:  Abstractie en algoritme
Bron: [het online platform van de Belgische Bebras-wedstrijd](https://bebras.ugent.be/)<br>
Tekst: Kris Coolsaet, BE<br>
Afbeeldingen: Kris Coolsaet, BE 

#### Toevalsprenten (Bebras ...)

De bevers hebben een klein bedrijfje dat gepersonaliseerde wenskaarten en geschenkpapier ontwerpt. De verschillende modellen worden gemaakt aan de hand van de volgende instructies:

1. Maak een cirkel C aan van een willekeurige kleur.
2. Herhaal de volgende stappen een willekeurig aantal keer.<br>
&nbsp;&nbsp;&nbsp;&nbsp;1. Maak een vierkant V aan van een willekeurige kleur en grootte.<br>
&nbsp;&nbsp;&nbsp;&nbsp;2. Kies een willekeurige grootte voor C: ofwel *klein*, ofwel *groot*.<br>
&nbsp;&nbsp;&nbsp;&nbsp;3. Druk C af, ergens op een willekeurige plaats.<br>
&nbsp;&nbsp;&nbsp;&nbsp;4. Druk V af, ergens op een willekeurige plaats.<br>

(Ter informatie: een vorm aanmaken betekent dat de vorm in het computergeheugen wordt aangemaakt, maar niet dat hij ook op papier wordt afgedrukt of getekend.)

*Welke van de volgende modellen werd niet door dit bedrijfje ontworpen?*

![Toevalsprenten](embed/bebrasabstractie2.png "Bebras Toevalsprent")

##### Oplossing

Het volgende model kan niet door dit bedrijfje zijn gemaakt:

![Toevalsprenten](embed/bebrasabstractie2oplossing.png "Bebras Toevalsprent oplossing")

##### Bespreking

Deze afbeelding bevat twee cirkels van verschillende grootte en van een verschillende kleur. In het algoritme wordt de kleur van de cirkel slechts één keer bepaald, namelijk helemaal in het begin; nadien kunnen de cirkels nog wel van grootte veranderen, maar niet van kleur.<br>
Alle andere antwoorden zijn mogelijke ontwerpen, ook al is dat misschien niet meteen duidelijk. Er moeten evenveel cirkels als vierkanten worden afgedrukt, maar het is best mogelijk dat een vierkant bovenop een cirkel wordt gedrukt en deze op die manier verbergt! Hou er ook rekening mee dat een cirkel of een vierkant toevallig dezelfde kleur kan hebben als de achtergrond.

Je moet het **algoritme** in voldoende mate kunnen toepassen. Als je inziet dat alle cirkels dezelfde kleur moeten hebben, dan heb je **abstractie** gemaakt van de instructies in het **algoritme**. Weten dat alle cirkels dezelfde kleur moeten hebben, is het enige dat van belang is om het antwoord te kunnen geven op de gestelde vraag. Je gebruikt eigenlijk slechts een deel van het algoritme. 
