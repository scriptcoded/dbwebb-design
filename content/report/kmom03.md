---
Title: Kmom03
Description: Redovisning kmom03.
Template: kmom
---

Redovisning kmom03
==========================

Jadå, nu kör vi! CSS-Grid och Flexbox! När jag började på min nuvarande
arbetsplats hade CSS-Grid nyligen börjat få en stabilt webbläsarstöd, så vi
valde att bygga med Flexbox istället. Jag har faktiskt aldrig byggt en "riktig"
sida med Grid, så det är skoj att få leka lite med det här. Det är ett väldigt
annorlunda tänk än vad man vanligtvis behöver när man håller på med
webbutveckling.

Jag flyttade runt mina SCSS-filer lite grann. Nu har jag tre "huvudfiler". De
använder sig utav partials i `scss/common` för att kunna ha lite mer struktur.
Jag gjorde lite arbete med att skriva om hur mina Twig-templates fungerar. Nu
har jag en `base.twig`-fil som fungerar som grund för alla andra Twig-filer.
Genom att använda `extends` slipper jag all boilerplate i mina olika layouts.
Det gör det även lättare att ändra saker globalt i framtiden. `extends` med
blocks är något som Twig har, men många andra templating engines saknar, så det
gjorde mig lite extra glad ^_^.

Idag har jag även valt att göra några andra ändringar än de ni föreslagit i era
texter. Först och främst valde jag att flytta min grid-kod från
`report/index.md` till min template-fil, eftersom det lät mig göra två saker.
Först och främst kunde jag använda `a`-taggar utan att Markdown wrappade dessa
med paragrafer. Sen kunde jag även använda Twigs loopar. Det gjorde i sin tur
att jag kunde ha en lista med kursmoment i `config/reports.yml`, och sedan loopa
över denna lista i både `report.twig` och `kmom.twig`. Smiiidigt! ^_^ Till slut
valde jag även att lägga tre responsiva lägen, dator, surfplatta och mobil. På
så vis kunde jag få det att se snyggt ut på alla skärmstorlekar. Någolunda
snyggt i alla fall...

Det var nog det för idag! TIL är att Pico har visat sig vara ett väldigt härligt
CMS, och Twig fungerar finfint som templating engine.
