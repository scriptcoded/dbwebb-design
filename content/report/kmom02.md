---
Title: Kmom02
Description: Redovisning kmom02.
Template: kmom
---

Redovisning kmom02
==========================

Gött, då var vi ingång med SCSS :) Kan börja med att säga att jag är gladd att
vi använder SCSS och inte SASS-syntaxen. Liksom, superduperglad. Jag har skrivit
min CSS med BEM-ish selectors, så det blev lite knasigt när Stylelint inte ville
låta mig använda dubbla understräck i klassnamn. Istället för att klydda runt
och installera extra Stylelintplugin stängde jag bara av den regeln. Jag gjorde
även några ändringar i NPM-projektet. Först och främst tog jag bort
`package-lock.json` från `.gitignore`. Som ni nämnde i kurstexterna så används
den för att låsa trädet, och då behöver den vara med i Git också. Har ni det så
pga. av någon annan teknisk anledning får ni hojta. Jag lade även till ett nytt
script, `npm run watch`. Kör bara SCSS med `--watch`-flaggan så att jag slipper
kompilera själv varje gång.

Hela mitt tema var redan skrivit med SCSS i bakhuvet. CSS-variabler ersätts lätt
med SCSS-variabler, och BEM funkar ganska med med SCSS. Jag orkade dock inte
skriva om alla filer till nästlade selectors. Tror bara att jag fixade
`header.scss`. Koden delade jag upp i grundfiler såsom `forms.scss` och
`elements.scss`, och större komponenter fick egna filer, t.ex. `header.scss` och
`footer.scss`.

TIL idag är att Stylelints VS Code-extension är trög.
