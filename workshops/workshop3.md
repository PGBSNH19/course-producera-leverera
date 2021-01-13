---
layout: page
title: Workshop
permalink: /workshops/workshop3
---

Refactor

**Torsdag den 14:e januari 2021**

Tidsplan:
* 9:30 start
* 15:00 samling och snak om typiska problem i har rakat på

I denna workshop ska ni också jobba med en annan grupps projekt.

Under dagen är det tanken att ni [refaktorera](../lectures/strategies#code-refactoring) koden för en annan grupp. När man refaktorera kan man göra det realtivt systmatisk, så tanken är att ni tar utgångpunkt i "31 Days of Refactoring", dock är hela listan lång, så fokusera enbart med dom 8 punkt som är listat här under. Primäre fokus ska vara på C# koden i APIet.

Ni får en branch (refactor-gX) som den som det är tänkt att ni jobbar emot. När ni är klara gör en pull request.

Vem gör vad:
* Grupp 1 refakturera Grupp 4
* Grupp 2 refakturera Grupp 1
* Grupp 3 refakturera Grupp 5
* Grupp 4 refakturera Grupp 3
* Grupp 5 refakturera Grupp 2

Hur kommer ni på gång:
1. Pull koden till eran lokala dator
1. Kör alla enhetstestar (säkerställ att dom är gröna)
1. Kör projektet lokalt (för att se att det funkar)
1. Påbörja refaktorering av API ut ifrån listen härunder (day 1 -> 7 + 30)
1. Medan ni refaktora notera följande:
    * Är der något specielt som har har fixat ett flertal gångar
1. Medan ni refaktora titta efter följande:
    * Potentiella säkerhets problem, gör i steg ett en kommentar i koden runt detta
    * Ställen vart man enkelt kunna lägga till enhetstestar
        * Det är såklart tillåten att implementera enhetstestar

## 31 Days of Refactoring

Full blogg serie: [31 Days of Refactoring](https://lostechies.com/seanchambers/2009/07/31/31-days-of-refactoring/)

Boken: [31 Days of Refactoring - Useful refactoring techniques you have to know](https://lostechies.com/wp-content/uploads/2011/03/31DaysRefactoring.pdf)

> Refactoring is an integral part of continually improving your code while it moves forward through time. Without refactoring you accrue technical debt, forget what portions of code do and create code that is resistant to any form of testing. It is an easy concept to get started with and opens the door to much better practices such as unit testing, shared code ownership and more reliable, bug-free code in general.

* [Day 1 : Encapsulate Collection](https://lostechies.com/seanchambers/2009/08/02/refactoring-day-1-encapsulate-collection/)
* [Day 2 : Move Method](https://lostechies.com/seanchambers/2009/08/02/refactoring-day-2-move-method/)
* [Day 3 : Pull Up Method](https://lostechies.com/seanchambers/2009/08/03/refactoring-day-3-pull-up-method/)
* [Day 4 : Push Down Method](https://lostechies.com/seanchambers/2009/08/04/refactoring-day-4-push-down-method/)
* [Day 5 : Pull Up Field](https://lostechies.com/seanchambers/2009/08/05/refactoring-day-5-pull-up-field/)
* [Day 6 : Push Down Field](https://lostechies.com/seanchambers/2009/08/06/refactoring-day-6-push-down-field/)
* [Day 7 : Rename (method, class, parameter)](https://lostechies.com/seanchambers/2009/08/07/refactoring-day-7-rename-method-class-parameter/)
* [Day 30 : Return ASAP](https://lostechies.com/seanchambers/2009/08/28/refactoring-day-30-return-asap/)

## Tools

Man kan få hjälp från verktyg som StyleCop:
* (https://github.com/DotNetAnalyzers/StyleCopAnalyzers)