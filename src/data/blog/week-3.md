---
author: Ho-Ping Keung
pubDatetime: 2025-10-19T15:22:00Z
modDatetime: 2025-10-19T16:52:45.934Z
title: Week 3
slug: week-3
featured: true
draft: false
tags:
  - code
  - exceptions
description:
 Temporal values
---

## Temporal Values

Tijdens het bekijken van mijn Dto’s ontdekte ik een concept dat ik nog niet eerder was tegengekomen TemporalValues. Dat prikkelde meteen mijn nieuwsgierigheid, want het leek duidelijk meer dan een gewone property. In deze blog deel ik wat ik ontdekte over TemporalValues

## Wat is een Temporal Model?

Een temporal model is een manier om data op te slaan die verandert doorheen de tijd. In plaats van telkens velden zoals startDate en endDate toe te voegen, zorgt een temporal model ervoor dat elke waarde automatisch gekoppeld wordt aan een periode waarin deze geldig is. Dit voorkomt rommelige work-arounds en geeft je domein een veel duidelijkere structuur.

Het sleutelelement hierin is de TemporalValue. Elke keer wanneer een waarde wijzigt, ontstaat er een nieuwe TemporalValue met zijn eigen geldigheidsperiode. Zo bewaart je applicatie niet alleen wat de actuele waarde is, maar ook wat die waarde vroeger was en wat ze zal worden.

Waarom TemporalValue gebruiken?

Temporal data opent de deur naar krachtige en natuurlijke features, zoals:

1. Versioned data

Data kan meerdere versies hebben, afhankelijk van de tijd.
Je kan vragen stellen als:

- “Welke prijs was geldig op 1 april?”

- “Welke waarde geldt vandaag?”

- “Wat zal de waarde zijn op 1 januari volgend jaar?”

Dit is bijzonder handig in domeinen zoals contractbeheer, verzekeringen, prijzen of HR-systemen.

2. Effective-dated domain modeling

Je model wordt veel overzichtelijker omdat je geen overal terugkerende velden zoals startDate of endDate meer nodig hebt. Het temporele systeem beheert automatisch welke waarden op welk moment geldig zijn.

3. Krachtige periode-gebaseerde queries

Temporal data maakt complexe tijdvragen eenvoudiger:

- waarden ophalen die een bepaalde periode overlappen

- opeenvolgende intervallen met dezelfde waarde automatisch mergen

- intervallen splitsen wanneer er binnen de geldigheidsperiode een verandering optreedt

Deze functionaliteit zorgt ervoor dat de data zichzelf correct gedraagt, ongeacht hoeveel wijzigingen er in de tijd plaatsvinden.

4. Automatische historische audit

Elke aanpassing creëert automatisch een nieuw “versie-record”.
Dat betekent:

- geen extra logging nodig

- volledige traceerbaarheid van alle historische wijzigingen

- perfecte audittrail out-of-the-box

In sectoren waar transparantie belangrijk is, zoals finance of juridische diensten, is dat een enorme meerwaarde.