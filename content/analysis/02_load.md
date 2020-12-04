---
Title: Analysis 02 Load
Description: Analysis 02 Load.
Template: kmom-analysis
---

Laddningstider hos högskole- och universitetshemsidor
=======================

Vi har analyserat tre hemsidor från olika svenska universitet/högskolor för att analysera deras laddningstider.

Urval
-----------------------

Vi valde två universitet och en högskola som alla har stort fokus på tekniska utbildningar, eftersom man bör kunna förvänta sig bra hemsidor från dessa. 

Metod
-----------------------
Sidorna skickades till pagespeed insights, som gav oss både ett betyg mellan 0-100 samt feedback på vad som skulle kunna göra att sidorna laddas fortare. Sedan användes devtools för att göra tre olika mätningar per sida av laddningstid, antal resurser och sidans storlek. Resultatet återfinnes i ett nedan länkat excel-ark. 

Resultat
-----------------------

### BTH

BTH behöver använda mer moderna filformat till sina bilder och reducera mängden oanvänd JavaScript på sin mobilhemsida. 

<div class="image-wrapper">
    <a href="%base_url%/image/analysis/kmom05/BTH.png" target="_blank">
        <img src="%base_url%/image/analysis/kmom05/BTH-780.jpg">
    </a>
    <div class="image-text">Blekinge Tekniska Högskolas hemsida</div>
</div>

### LTU

De skulle kunna spara ca 5 sekunder på att optimera sina bilder.

<div class="image-wrapper">
    <a href="%base_url%/image/analysis/kmom05/LTU.png" target="_blank">
        <img src="%base_url%/image/analysis/kmom05/LTU-780.jpg">
    </a>
    <div class="image-text">Luleå Tekniska Universitets hemsida</div>
</div>

### LIU

De skulle kunna spara ca 4 sekunder på att ta bort JavaScript-kod som inte används, framförallt YouTube-spelaren.

<div class="image-wrapper">
    <a href="%base_url%/image/analysis/kmom05/LIU.png" target="_blank">
        <img src="%base_url%/image/analysis/kmom05/LIU-780.jpg">
    </a>
    <div class="image-text">Linköpings Universitets hemsida</div>
</div>

Excel-ark: https://docs.google.com/spreadsheets/d/1szMszEo4tsNvL_pjnmSW9BPmonXNYUlVQA0HmHEudh4/edit?usp=sharing

Analys
-----------------------

Alla tre sidor presterar bättre på desktop än på mobil. BTH och LTU led båda av problem med bildoptimering. Troligen är bilderna sämre anpassade för mobil än desktop. Eftersom mobiler har sämre nätverk kräver de att bilderna är mindre.

LIUs hemsida laddar in icke-essentiella saker innan det relevanta innehållet. En enkel åtgärd är att se till att javascriptfilen laddas in längst ner i html-dokumentet. 

### Vår rankning

På första plats kommer LTU med ett snitt på 2,14 sekunder i laddningstid. LTU är den sida som hämtar flest resurser. De håller dock nere sin laddningstid och storlek eftersom majoriteten av resurserna endast är på deras universitetsprogramsida, och är små data om respektive program, exempelvis namn och program-ID. 

På andra plats kommer BTH med ett snitt på 2,26 sekunder i laddningstid. De får diplom för att de laddar in färst resurser.

På tredje plats kommer LIU med ett snitt på 3,18 sekunder i laddningstid. De har även sämst resultat gällande både PageSpeed Insights-betyg och sidstorlek.

### Upplevelse av laddningstid

Enligt Jakob Nielsen (1993) så tappar användaren fokus när en hemsida laddar i över 10 sekunder. Vi håller med om detta, när en sida tar ca 10 sekunder på sig att ladda kommer impulsen att lämna sidan. Samtliga analyserade sidor klarar denna gräns, även med simulerad snabb 3G-uppkoppling.

När man öppnar skolans förstasida upplevs BTHs hemsida som snabbast. Det kan bero på att den har en bakgrundsvideo som laddas fort. Den lockar till sig blicken och distraherar användaren. Vi upplever att LIUs hemsida är snabbare än de andra när man klickar runt bland hemsidans undersidor. Detta skiljer sig från våra testresultat, men dessa täcker endast initiell laddning av hemsidorna. LIUs hemsida skulle t.ex. kunna vara bättre på att återanvända nedladdade resurser med hjälp av caching.

Referenser
-----------------------
PageSpeed Insights: https://developers.google.com/speed/pagespeed/insights/

Jakob Nielsen (1993). Response Times: The 3 Important Limits (https://www.nngroup.com/articles/response-times-3-important-limits/)

Övrigt
-----------------------

Vi som skrivit rapporten heter Molly Andersson, Malcolm Nihlén och Veronica Axelsson.
