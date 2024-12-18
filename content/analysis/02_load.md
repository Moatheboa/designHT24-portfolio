---
Title: Load
Description: Load
Template: analysis-pages
---

Laddningstider
=======================

En analys av tre olika hemsidors laddningstider.

Urval
-----------------------
IKEA:  
<picture class="loadPhotos">
    <source media="(min-width: 768px)" srcset="%base_url%/image/ikea.png?w=600&save-as=jpg">
    <img src="%base_url%/image/ikea.png&w=300" alt="Ikea's webpage">
</picture>  

A: Förstasida: https://www.ikea.com/se/sv/  
B: Cirkulärbutik: https://www.ikea.com/se/sv/circular/second-hand/  
C: Planeringsverktyg: https://www.ikea.com/se/sv/planners/  
<br>
BILTEMA: 
<picture class="loadPhotos">
    <source media="(min-width: 768px)" srcset="%base_url%/image/biltema.png?w=600&save-as=jpg">
    <img src="%base_url%/image/biltema.png&w=300" alt="biltema's webpage">
</picture>  

A: Förstasida: https://www.biltema.se/  
B: Båtsida: https://www.biltema.se/bat/  
C: Verktyg: https://www.biltema.se/verktyg/  
<br>
BYGGMAX:  
<picture class="loadPhotos">
    <source media="(min-width: 768px)" srcset="%base_url%/image/byggmax.png?w=600&save-as=jpg">
    <img src="%base_url%/image/byggmax.png&w=300" alt="Byggmax's webpage">
</picture>  
A: Förstasida: https://www.byggmax.se/  
B: Fönster och dörrfärg: https://www.byggmax.se/farg-och-tapeter/utomhusfarg/fonsterfarg-och-dorrfarg  
C: Förvaringslådor: https://www.byggmax.se/inredning/forvaring/forvaringslador


Metod
-----------------------

För att mäta laddningstider har verktyget PageSpeed Insights från Google använts för att kolla hemsidornas olika sidors URL:er i mobile och desktop mode.  
Sedan har jag laddat om varje sida tre gånger och noterat värden för antal begäran, storlek samt load från fliken nätverk hos Firefox Devtools.

Resultat
-----------------------
M: Mobile  
D: Desktop  
LCP: Largest Contentful Paint  
INP: Interaction to Next Paint  
CLS: Cumulative Layout Shift  
FCP: First Contentful Paint  
TTFB: Time To First Byte  
*: Genomsnitt av tre laddningar.  
Anmärkningar: Ifall sidan ej godkändes av PageSpeed Insights och isf vilken kategori som var för långsam.  

<div class="embed-container">
    <iframe src="https://docs.google.com/spreadsheets/d/e/2PACX-1vRc_ciLDhE--jgmevZl-UcbO0Q-imlZ8pOH7CYCbsNOyd1Nr1zI6V6s8dBwUURkCUoperSK3OWx6yVa/pubhtml?widget=true&amp;headers=false"></iframe>
</div>

Analys
-----------------------

Alla tre hemsidorna hade flera sidor som inte blev godkända av PageSpeed Insights.  
Byggmax var den sämsta, där var det bara desktop-varianten av förstasidan som fick godkänt. På de andra fallerade tiden på CLS, och i ett fall TTFB. Byggmax hade kortast load-tid, men på sidorna som inte var första-sidan var TTFB-tiden rätt usel. Byggmax hade också generellt längre tid på LCP, CLS och FCP.  
Biltemas förstasida blev underkänd, både mobile och desktop mode på grund av för långsam CLS. Alla biltemas sidor hade ganska få resurser, ca 40 jämfört med Ikea's och Byggmax över 150. I övrigt var Biltema och Ikea ganska samma utöver att Ikeas totala storlek var större på alla sina sidor.  
Ikea blev också underkänd på en av sina sidor. I mobilversionen var det INP som var för långsamt och i desktopversionen CLS.  
Jag tänkte först tilldela guldplatsen till Ikea, främst för att jag tycker att det är extra viktigt att förstasidan fungerar bra. Men upplevelsen när jag besöker sidorna är ändå att Biltemas snabbare, och den har ju också bättre load. Så Biltema vinner i användarupplevelse!  
Jag är inte så otålig så tycker alla tre hemsidor laddar tillräckligt snabbt för mig. Men har man en sämre internetuppkoppling eller segare dator så vill man såklart ha det snabbare. Då kanske 2s är en lämpligt gränsvrde för en bra tid. Då klarar Ikea sig inte.


Referenser
-----------------------

Hemsidorna specificerade ovan samt PageSpeed Insights och Firefox Devtools.

Övrigt
-----------------------

Av Moa Karlsson.