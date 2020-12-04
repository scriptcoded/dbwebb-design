---
Title: Kmom05
Description: Redovisning kmom05.
Template: kmom
---

Redovisning kmom05
==========================

Det var intressant att se att så många webbplatser led av problem med
bildstorlek, framförallt eftersom att de hemsidor vi tittade på tillhörde
universitet och högskolor med teknisk spets. Utöver bilder var även ett
genomgående problem att mycket onödiga resurser skickades på mobilsidorna.

Det är mycket skönare att kunna låta servern göra arbetet åt en. Bildhantering
är ändå mest jobbigt. Det finns dock fall då man t.ex. vill beskära en bild på
ett specifikt sätt, t.ex. för att inte klippa ett huvud på mitten. Då kommer
lite manuellt arbete till nytta. Jag brukar använda GIMP och InkScape då jag
sitter på Linux.

Tar man inte bilder i beaktskap blir det lätt tunga sidor. Använder man ett
ramerk eller CMS som är lite smart slipper man tänka på det och får bilder i
rätt storlek automatiskt. Ska man utveckla något åt någon annan, t.ex. ett
CMS-tema, så kan det vara bra att ha bilder i åtanke.

TIL idag är <code>&lt;picture&gt;</code>. Har faktiskt aldrig använt det innan,
utan har bara använt <code>srcset</code>.

Jag valde idag att använda en loop som itererar över metadata i min Markdownfil
för att rendera galleriet. På så sätt kan jag skapa fler galleri i framtiden.
Jag skapade även en SCSS-mixin för hovringsbara element, t.ex. bilderna i
galleriet.

Här kommer mina två videor :)

<div class="embed-wrapper">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/HPk-VhRjNI8" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>

<br>

<div class="embed-wrapper">
    <iframe width="560" height="315" src="https://www.youtube.com/embed/jl0TWPvKluk" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</div>
