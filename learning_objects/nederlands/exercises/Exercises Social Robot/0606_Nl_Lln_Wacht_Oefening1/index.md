---
hruid: sr_WachtOef1
version: 3
language: nl
title: "Oefening Wacht 1"
description: "Oefening Wacht 1"
keywords: ["StartTodwenguino", "wacht"]
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
estimated_time: 5
skos_concepts: [
    'http://ilearn.ilabt.imec.be/vocab/curr1/s-computers-en-systemen'
]
teacher_exclusive: false
---

### Oefening Wacht

OPGAVE 1

Schrijf een programma dat het volgende doet:

* Laat "Hallo mensen" op het lcd-scherm verschijnen gedurende 1 seconde (1000 ms).
* Laat "Ik ben dwenguino" op het lcd-scherm verschijnen voor 2 seconden (2000 ms).

Het *'wacht'-blok* dat **na** een bepaalde instructie staat, geeft weer hoelang de computer moet **wachten** vooraleer deze met de volgende instructie mag beginnen.

