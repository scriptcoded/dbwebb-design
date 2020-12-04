---
Title: Kmom04
Description: Redovisning kmom04.
Template: kmom
---

Redovisning kmom04
==========================

Att få göra en gruppavgift var roligt. Vi dök djupt ner i våra olika sidor, och
hittade massor mer intressanta lik- och olikheter än vad uppgifter omfattade.
Det var faktiskt en betydligt roligare uppgift än vad jag förväntat mig!

Jag valde att använda mig av ett komplementärt färgschema. Basfärgen är
<code style="color: #fff; background-color: #d41948;">#d41948</code> och
komplementfärgen <code style="color: #fff; background-color: #18a82b;">#18a82b</code>.
Hela paletten ser ut som följande:

<table class="swatch-table">
 <tr>
   <td style="background-color: #870828"></td>
   <td style="background-color: #ff386a"></td>
   <td style="background-color: #d41948"></td>
   <td style="background-color: #008713"></td>
   <td style="background-color: #19d434"></td>
 </tr>
</table>

Primärt är sidan ljus (eller mörk i dark mode). Basfärgen
<code style="color: #fff; background-color: #d41948;">#d41948</code> används
lite här och var för att dra uppmärksamhet, och även
<code style="color: #fff; background-color: #18a82b;">#18a82b</code> används på
t.ex. [Report](%base_url%/report) och [Analyses](%base_url%/analysis).

Dark mode löste jag genom att bryta ut mina stylefiler till imports som sedan
kunde importeras efter olika variabeldeklarationer. Som exempel så tog jag
`style.scss` och flyttade till `_style.scss`. Jag bröt ut importen för variabler
och lade i `style.scss` och `style-dark.scss`. I den sistnämnde importerade jag
även en extra variabelfil, `_variables-dark.scss`, som innehåller extra
variabler som trumfar de vanliga och gör sidan mörk. Eftersom att all CSS redan
använde variabler var det en enkel sak att bryta ut. För att byta mellan de
olika varianterna använde jag koden för sessionen som fanns att tillgå, och lade
en knapp för att byta mellan dessa i toppmenyn. Beroende på vilket läge som är
valt så importeras olika CSS-filer i headern. Denna kod finns även i de
layoutfiler som använder egna stylefiler, t.ex. `kmom.twig`.

TIL idag är att hantera teman i SCSS fungerar, men det vore betydligt lättare
med CSS-variabler. Men då tappar vi en stor del av SCSS.
