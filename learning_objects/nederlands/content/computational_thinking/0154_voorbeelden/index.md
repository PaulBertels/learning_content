---
hruid: ct_voorbeelden4
version: 3
language: nl
title: "Literatuur over CD en wetenschappen"
description: "Literatuur over CD en wetenschappen"
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
# Integreren van computationeel denken en handelen in lessen wetenschappen en wiskunde 

Veel onderzoekers hebben in wetenschappelijke artikels gepubliceerd welke mogelijkheden zij zien om computationeel denken en handelen in bestaande lessen te laten aan bod komen. 

We geven hier een (niet exhaustief) overzicht.

**Barr en Stephenson (2011)** benadrukken dat de ontwikkelingen in de computerwetenschappen ervoor zorgen dat probleemoplossend denken een nieuwe insteek krijgt en dat oplossingen op een nieuwe manier kunnen uitgetest worden.<br>

|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Data verzamelen|gegevensbron vinden voor een probleem|gegevens verzamelen via experiment uit kansrekenen, bv. gooien met dobbelstenen of munten opgooien|gegevens verzamelen via experiment|
|Data analyse|programma schrijven om eenvoudige statistische berekeningen te doen op een dataset|aantal keer kop of munt automatisch laten tellen en resultaat interpreteren|gegevens analyseren van een experiment|
|Data voorstellen|gegevensstructuren gebruiken zoals array, gekoppelde lijst, stack, wachtrij, grafiek, hash tabel, enz.|histogram, taartdiagram, staafdiagram gebruiken om gegevens weer te geven; stel gegevens overzichtelijk voor d.m.v. verzamekingen, lijsten, grafieken, enz.|gegevens samenvatten van een experiment|
|Abstractie|een reeks van vaak herhaalde instructies abstraheren tot een functie|het gebruik van letters in algebra; in een vraagstuk de nodige gegevens eruit halen|een model bouwen van een fysieke entiteit|
|Modellen valideren| |regressielijnen|model toetsen aan de werkelijkheid|
|Simulatie|animatie van een algoritme, parameters meerdere waarden laten aannemen om effect te zien|effect van de waarde van de parameters bij een functie bestuderen op een grafiek|beweging van het zonnestelsel simuleren|
|Automatisatie||eenvoudige zaken in Python programmeren; Geogebra gebruiken| |
|Testen en evalueren|programma debuggen|antwoord schatten en verifiëren|data opkuisen| | |
|Algoritme|bestudeer klassieke algoritmen; een algoritme voor een probleem|staartdeling uitvoeren, ontbinden in factoren, cijferen|een experimentele procedure uitvoeren|
|Decompositie|objecten en methoden definiëren; hoofddeel programma afbakenen en functies definiëren|volgorde van bewerkingen in een uitdrukking toepassen|een soortenindeling maken|
|Controlestructuren|controlestructuren gebruiken conditionals, lussen, recursie, enz.|wiskundige functies bestuderen vergeleken met functies in programmeren; iteratie gebruiken om vraagstukken op te lossen||
|Parallelisatie|*threading*, *pipelining*, het verdelen van gegevens of taak op zo'n een manier om te worden verwerkt in parallel|stelsel van lineaire vergelijkingen oplossen; matrixvermenigvuldiging|data opkuisen|experimenten gelijktijdig uitvoeren met verschillende parameters|

**Bocconi et al. (2016) geven voorbeelden van computationeel denken binnen maar ook buiten STEM-vakken.** <br>
**Taub 2014 Yevseyeva 2012**

|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Programmeren|videogames maken via programmeren in Scratch|||
|Abstractie|||verschillende niveaus van abstractie bij het oplossen van een probleem uit de fysica| 

**Weintrop et al. (2015) focussen op CD in lessen wiskunde en wetenschappen.**

|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|------------|----------------------------|
|Simuleren|Sim2Real|model gebruiken; Netlogo|model gebruiken; Concord Consortium's Molecular Workbench; PhET-project; Netlogo; iLab Network|
|Modelleren|Sim2Real|model creëren|model creëren|
|Data genereren||microcontroller|microcontroller|
|Data voorverwerken|gegevens sorteren, filteren, opkuisen, normaliseren, samenbrengen|||
|Programmeren|bestaande programma's begrijpen en/of aanpassen, functies schrijven|data visualiseren, wiskundige model bouwen||  
|Inzicht in tools|sterktes en zwaktes van digitale tools kunnen afwegen t.o.v. elkaar|||
|Abstractie||door iets abstract voor te stellen meer duidelijkheid bieden|door iets abstract voor te stellen meer duidelijkheid bieden|
|Evalueren en debuggen|strategieen om uit te vissen waarom iets niet werkt zoals verwacht|||
|Systeemdenken|||analyse van de interactie tussen de verschillende delen van een syteem en het geheel, zoals bij natuurlijke selectie, dynamiek binnen een populatie, ademhalingsstelsel, ideale gaswetten; cross-cutting concepts zoals feedback en stromen beter begrijpen a.d.h.v. digitale tools|
|Decompositie|||de verschillende delen van een syteem kunnen idientificeren en hun interacties beschrijven|de verschillende delen van een syteem kunnen idientificeren en hun interacties beschrijven|
|Denken in niveaus|||hoe veranderingen op microniveau leiden tot verabderingen op macroniveau|
|Communiceren|||infographic|

Men kan bv. datasets vinden op het world wide web, maar om uit die data conclusies te kunnen trekken is er voorbereidend werk nodig. Deze data moeten worden opgekuist, eventueel verwerkt en op een geschikte manier worden voorgesteld. Leerlingen moeten over de conclusies leren communiceren. AI-systemen zoals deep learning werken met zeer grote datasets. Het is belangrijk dat leerlingen begrijpen hoe deze grote datasets tot stand komen, en hoe beperkingen in de dataset leiden tot tekortkomingen van de AI-systemen, zoals de aanwezige bias.

Leerlingen kunnen ook zelf data genereren via een experiment, bv. gebruikmakend van een microcontroller.

Als men modellen gebruikt om een simulatie te doen, dan is het belangrijk dat men meegeeft wat de beperkingen en de voordelen zijn van een simulator.

Je kan de leerlingen problemen voorschotelen die uitermate geschikt zijn om met de computer aan te pakken. Soms kan dat door problemen uit bestaande lessen wat te herformuleren, rekening houdend met bv. de tools die de leerlingen kunnen gebruiken. Leerlingen kunnen leren welke soort tool geschikt is voor welke taak.

Leerlingen leren dat alles als een systeem kan bekeken worden.

**Lowe & Brophy (2017)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|------------|----------------------------|
|Algoritme|doolhof doorlopen|||

**Lu & Fletcher (2009)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|------------|----------------------------|
|Data voorstellen||Computationele voor- en nadelen soort diagram||
|Iteratie||Vermenigvuldiging als iteratieve optelling||
|Abstractie||Vergelijking||
|Algoritme||Algoritme voor het trekken van een vierkantswortel||

**Grover & Pea (2017)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|------------|----------------------------|
|Logica||logische uitdrukkingen in een real-world context||
|Patroonherkenning|gezichtsherkenning op Facebook en aanbevelingen op Amazon of iTunes|||
|Abstractie|algoritme als voorbeeld van abstractie|model en simulatie als abstractie van fenomeen in de echte wereld||
|Automatisatie|wanneer is automatisatie zinvol; nodige abstracties en datarepresentaties|||
|Decompositie|zich klaarmaken voor school bestaat uit verschillende taken die elk weer bestaan uit subtaken|gemiddelde berekenen van de klas voor een examen (wat is er nodig)||
|Artefact|programmeren en simuleren gevolgd door fysieke artefact; programmeren van een app bruikbaar door anderen|||

**Berry (2021a) en (2021b)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Abstractie|||verschillende niveaus van abstractie van aardrijkskundige kaarten| 
|Decompositie|technische opdracht verdelen in subtaken||| 
|Programmeren|nadenken over sequentie, iteratie, selectie, variabelen, invoer en uitvoer||| 

**Cansu et al. (2019)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Abstractie||Om een 'vraagstuk' op te lossen, moeten leerlingen relevante zaken van niet-relevante van elkaar onderscheiden en komen tot een op te lossen vergelijking|abstractie van aardrijkskundige kaarten| 
|Patroonherkenning en generalisatie|subprogramma (functie)||| 

**Mishra & Yadav (2013)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Parameters|experimenteren met de parameters in een logo om nieuwe logo's te creëren|parameters in een logo identificeren||

**Lee et al. (2011)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Abstractie en automatisering|ontwerpen en programmeren van webpagina's en smartphone-apps||| 
|Modelleren en simuleren, en abstractie|Selecteren van de kenmerken die opgenomen worden in een model|||
|Abstractie|Robot ontwerpen die aan bepaalde criteria moet beantoowrden|||
|Automatiseren|Programma verwerkt invoer van de sensoren op een robot|||

**Yadav et al. (2016)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Data analyseren|||internationale datsets van broeikasgasuitstoot vergelijken naar hoeveelheid, land, economische sector ...| 
|Abstractie, modelleren||model van ons zonnestelsel maken|
|Abstractie, simuleren||simuleren hoe bevolking regaeert op een ziekte-uitbraak|
|Automatisatie, modeleren en simuleren||simuleren a.d.h.v. Netlogo om patronen op te sporen biologische, aardrijkundige, fysische, chemische ... processen|

**Lee & Malyn-Smith (2019)**
|**CD**|**Computerwetenschappen**|**Wiskunde**|**Natuurwetenschappen**|
|---------------|------------------------|-----------|----------------------------|
|Algoritme|10 000 items sorteren|werken met grote hoeveelheden data|voorbeelden geven van systemen die veel rekenkracht vergen, zoals weermodellen|
|Algoritme|robot die een pad volgt||robot volgt een pad dat de metamorfose van rups tot vlinder weergeeft in de juiste volgorde|
|Algoritme||flowchart maken in een les over delers en veelvouden|wetenschappeleijke redenering verwoorden m.b.v. als-dan constructie, bv. om een hypothese te evalueren|
|Decompositie|uitzoeken hoe een bestaand Legobouwsel geconstrueerd werd||uitzoeken hoe een simulatietoepassing werkt|
|Abstractie|RGB als abstractie van het aantal kleuren dat mensen kunnen waarenemen|keuze paramaeters die meegenomen worden in een wiskundig model|leerlingen maken een schema van een gegeven elektronische opstelling en andere leerlingen construeren de opstelling opnieuw a.d.h.v. het schema|
|Abstractie|representatie opmaken die kan geprogrammeerd worden||beslissingsboom voor classificatie opstellen; algebraïsche functie schrijven voor een proces|
|Programmeren|toestel ontwerpen en bouwen om paperclips te tellen|geld wisselen; bewegen op een getallenlijn (bv. in Scratch)||
|Data|data verzamelen (via dataloggers, via world wide web, via simulaties) en opkuisen|kansverdeling simuleren|data verzamelen (via dataloggers, via world wide web, via simulaties), opkuisen, monitoren en analyseren; meedoen aan een citizen science project|
|Automatisatie|bespreken welke dagdagelijkse processen er (deels) geautomatiseerd kunnen worden en welke niet|stelsels vergelijkingen laten oplossen door de computer|simulaties gebruiken, bv. betreffende de dynamiek in een ecosysteem|



