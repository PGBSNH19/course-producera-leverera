---
layout: page
title: Ask Almost Anything
permalink: /aaa/
---

Följande frågor har ställs tillsvidre:
* Design pattern för console applikationer. Alltså separerea gui med logic/model. 
    * Dependency injection, eller ej? 
    * Kod exempel
    * Kanske en modelclass för logik, en guiclass och sedan hur man sammanflätar detta på ett stabilt och bra sätt.
* Data access mellan razorpages alltså cshtml till cshtml.cs. Samt andra bas steg, som du anser skapar en god grund. 
    * Med kodexempel
* Med CD så pratas det om att deploya mjukvara ofta. Vissa nämner även att man kan deploya så att användarna inte ens märker något. 
    * Är det något speciellt som man behöver göra då eller är det bara att en push kan gå så snabbt så i värsta fall får användaren ett error men klickar igen på länken så funkar det.
* Microservices
    * Hur funkar det? 
    * Finns det standarder? 
    * Är det mer eller mindre att man lägger olika Controllers och tillhörande Repositories i ett egen API med egen databas? 
    * Blir det inte extremt mycket mer trafik via HTTP?
* Tips på att hosta Container Images, Databaser, Storage billigt. 
    * (Detta har vi gått igenom men tycker fortfarande att det är svårt, speciellt när man betalar $0.00012 per CPU sekund eller dylikt)
* Single Responsibility Principen
    * En metod ska göra en sak. Men vad är en sak (Det verkar vara lite delade åsikter i just detta) ? 
    * Låt oss säga att du ska ladda upp en fil till en webserver. Då kanske du behöver:
        1. Kolla så att Directory finns
        1. Spara filen
        1. Skriva något till en databas
* Container orchestration
    * Kubernetes
    * Docker swarm