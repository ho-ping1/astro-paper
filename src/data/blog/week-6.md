---
author: Ho-Ping Keung
pubDatetime: 2025-10-19T15:22:00Z
modDatetime: 2025-10-19T16:52:45.934Z
title: Week 6
slug: week-6
featured: true
draft: false
tags:
  - code
  - git
description:
 Git version control
---

## Git version control

Tijdens de zesde week van mijn stage kwam ik voor een onverwachte uitdaging te staan, eentje die me uiteindelijk heel wat heeft bijgeleerd over Git en het belang van proper branch-beheer. Ik had namelijk een grote fout gemaakt: ik was vergeten mijn branches regelmatig up-to-date te houden met de master.

Dat probleem kwam pas echt aan het licht toen mijn stagebegeleider mijn werk wilde nakijken en dat simpelweg niet kon, omdat mijn branches achterliepen op de nieuwste wijzigingen. Oude code, conflicten, ontbrekende updates allemaal omdat ik mijn branches niet regelmatig had gesynchroniseerd.

Wat ik heb bijgeleerd
1. Het belang van stashing

Ik ontdekte hoe waardevol git stash eigenlijk is. In plaats van half-afgewerkte code zomaar te committen of te verliezen, kon ik mijn wijzigingen tijdelijk wegzetten. Dit gaf me de ruimte om mijn branch netjes bij te werken zonder bang te zijn dat ik werk zou kwijtraken.

2. Cherry-picken als reddingsmiddel

Sommige commits zaten in de verkeerde branch, of waren al deels opgelost op master. Met git cherry-pick kon ik specifieke commits overnemen zonder de rest van de rommel mee te sleuren. Dit gaf me veel meer controle tijdens het opschonen.

3. Up-to-date blijven is geen luxe, maar noodzaak

De grootste les?
Als je branches niet bijhoudt, maak je je eigen leven (en dat van je begeleider) onnodig moeilijk. Regelmatig pullen, rebasen of mergen voorkomt dat je dagen moet spenderen aan fouten oplossen die nooit hadden moeten bestaan.

Conclusie

Hoewel het even slikken was toen ik besefte hoeveel werk mijn fout veroorzaakte, ben ik blij dat het gebeurd is. Door mijn branches op te kuisen heb ik veel geleerd over:

- stashing

- cherry-picking

- het correct synchroniseren van branches

- en vooral: discipline in versiebeheer

Het was een technische wake-upcall die me nu al helpt om veel efficiënter en professioneler met Git te werken.