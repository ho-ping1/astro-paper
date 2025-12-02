---
author: Ho-Ping Keung
pubDatetime: 2025-10-19T15:22:00Z
modDatetime: 2025-10-19T16:52:45.934Z
title: Week 7 & 8
slug: week-7 & 8
featured: true
draft: false
tags:
  - code
  - git
  - exceptions
description:
 Verbetering code
---

## Verbetering code

Tijdens de weekend heeft mijn begeleider naar mijn code gereviewed zodat ik het tijdens de 7de week kon verbeteren. Een van de fouten was git gerelateerd waarbij ik een LocalModule file had dat gepushed werd maar wat niet de bedoeling was. Ik moest dus een gitignore aanmaken zodat dat het niet meer mee gepushed werd. Verder had ik ook "dead" code laten liggen in de branch. Dat is code dat ik geschreven heb maar uiteindelijk niet gebruikt heb maar ben dan vergeten om het te verwijderen uit de code. Andere fouten bestond uit het de opdracht goed verstaan waardoor de code niet doet wat het zou moeten doen, NullExceptions en functies dat ik over het oog heb gezien en niet geimplementeerd waren.

Nog een error dat ik kreeg was dat ik soms na het updaten mijn schema's up to date waren omdat er nieuwe kollomen waren toegevoegd aan de database. Dus moest ik liquibase updaten. Deze library zorgt voor de tracking en managing van de database schema's zodat ze niet achterlopen via scripts.