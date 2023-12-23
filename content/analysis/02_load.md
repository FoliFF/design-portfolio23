---
Title: Load
Description: Rapport för laddningstid.
---
Load
=======================

Denna analys fokuserar på att utvärdera laddningstid och användbarhet för tre utvalda webbplatser. Syftet är att identifiera och jämföra hur dessa webbplatser presterar i termer av hastighet och interaktion, vilket ger insikter i deras övergripande effektivitet och tillgänglighet.

Urval
-----------------------

I denna analys kommer jag att fokusera på tre specifika webbplatser: Chalmers Tekniska Högskola, Blekinge Tekniska Högskola och Skatteverket. Valet av dessa webbplatser grundar sig på en önskan att undersöka och jämföra prestanda och användbarhet mellan akademiska institutioner och en statlig myndighet.
### Motivering till urvalet:
Akademiska Webbplatser: Chalmers Tekniska Högskola och Blekinge Tekniska Högskola representerar två av Sveriges framstående tekniska universitet. Deras webbplatser förväntas reflektera moderna webbdesignstandarder och vara optimerade för en mångsidig användargrupp, inklusive studenter, forskare och lärare. Genom att analysera dessa två webbplatser kan vi få insikter i hur högskolor använder webbdesign för att möta behoven hos en bred och mångfaldig publik.
Statlig Myndighetswebbplats: Skatteverkets webbplats representerar en annan kategori av webbplatser med en betydande roll i det offentliga rummet. Som en myndighetswebbplats har den unika krav på tillgänglighet och informationstillhandahållande till allmänheten. Analysen av Skatteverkets webbplats ger en kontrast till de akademiska webbplatserna och visar hur en statlig myndighet hanterar sina digitala resurser.
Denna jämförelse mellan akademiska institutioner och en statlig myndighet ger en bredare förståelse för hur olika organisationer tillämpar webbdesign och teknik för att uppfylla sina specifika mål och användargrupper.


Metod
-----------------------

För att analysera webbplatsernas laddningstid och användbarhet kommer jag att använda Google PageSpeed Insights och webbläsarens DevTools. Dessa verktyg erbjuder omfattande data och insikter som hjälper till att bedöma webbplatsens prestanda och användarvänlighet.
### PageSpeed Insights
Användning: PageSpeed ger en detaljerad analys av hur snabbt en webbplats laddar på både mobila enheter och stationära datorer. Det ger en övergripande poäng baserad på flera faktorer som påverkar webbplatsens prestanda.
Datainsamling: För varje webbplats kommer jag att registrera PageSpeed-poäng för både mobila och stationära versioner. Jag kommer också att notera specifika rekommendationer och varningar som PageSpeed ger, vilket kan ge insikter i potentiella förbättringsområden.
### DevTools (Network Tab)
Användning: DevTools Network-fliken ger en detaljerad tidsförlopp av sidans laddningsprocess. Den visar alla nätverksförfrågningar som webbsidan gör, inklusive filstorlekar och laddningstider.
Datainsamling: Jag kommer att använda DevTools för att mäta total laddningstid, antalet resurser som laddas (till exempel bilder, CSS-filer, JavaScript-filer) och sidans totala storlek. För varje sida kommer jag att göra tre mätningar

Resultat
-----------------------


<div class="embed-container">
  <iframe width="700" height="400" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQv05aYqi2AwFz8-iwUuskk8EfDGk-dIY2xtLwQ0ESDB91TaYYzEQClTvIzqH7hVvHYT96y5WLY6sEH/pubhtml" title="Web result" frameborder="0" allowfullscreen></iframe>
</div>


#### Chalmers Tekniska Högskola
 •	<strong>Mobil:</strong> PageSpeed Insights ger betyget 73 för prestanda. Viktiga mätvärden inkluderar Largest Contentful Paint (LCP) på 1,7 sekunder och Time to First Byte (TTFB) på 0,9 sekunder.
•	<strong>Desktop:</strong> Prestationsbetyget är 94, med ett LCP på 0,9 sekunder och TTFB på 0,4 sekunder.
•	<strong>DevTools:</strong> Mätningar visade att sidan laddar i genomsnitt på 635 ms med 80 resurser som laddas och en total storlek på 0,966 MB överförda data.
#### Blekinge Tekniska Högskola
•   <strong>Mobil:</strong> PageSpeed Insights visar ett prestandabetyg på 91, med ett LCP på 2,4 sekunder och ett TTFB på 1,6 sekunder.
•   <strong>Desktop:</strong> Betyget för prestanda är 94, med ett LCP på 1,7 sekunder och ett TTFB på 1,3 sekunder.
•   <strong>DevTools:</strong> Genomsnittlig laddningstid är 1,08 sekunder för sidan med 86 resurser som laddas och en total storlek på 2,2 MB överförda data.
#### Skatteverket
•   <strong>Mobil:</strong> Ett lågt prestandabetyg på 52 från PageSpeed Insights, med ett LCP på 2,2 sekunder och ett TTFB på 0,4 sekunder.
•   <strong>Desktop:</strong> Prestationsbetyget ökar till 72, med ett LCP på 1,4 sekunder och ett TTFB på 0,2 sekunder.
•   <strong>DevTools:</strong> Sidan laddas i genomsnitt på 657 ms med 42 resurser som laddas och en total storlek på 1,7 MB överförda data.

Analys
-----------------------

Chalmers uppvisar hög prestanda på båda plattformarna, medan BTH visar större variation. BTHs mobila LCP är längre, vilket kan påverka användarupplevelsen. Chalmers är snabbare på desktop, vilket antyder bättre optimering för stationär användning.
DevTools visar att Chalmers har kortare laddningstider och större datamängd, vilket kan indikera högkvalitativt innehåll. För BTH finns det utrymme för optimering baserat på mobila laddningstider.
Skatteverket har längre LCP på mobil, vilket försenar synligt innehåll för användaren. Även om desktop-prestandan är bättre, behöver den synliga innehållsladdningen förbättras.
Sammanfattningsvis kan användarupplevelsen på alla tre webbplatserna förbättras, särskilt för mobila användare. Regelbunden optimering är viktig för att möta användarförväntningarna om snabba laddningstider.
DevTools Nätverkspanelens resultat bekräftar webbplatsens effektivitet med en snabb laddningstid och måttlig resursladdning. Dock kan den längre tiden för DOMContentLoaded-händelsen jämfört med den totala laddningstiden peka på möjlig JavaScript-exekvering som påverkar interaktiviteten.
För att förbättra användarupplevelsen, särskilt på mobila enheter, bör fokus ligga på att minska LCP och noggrant granska JavaScript-exekveringen för potentiella optimeringar. Att minska resursstorlek och antal genom komprimering och försiktig skriptladdning kan leda till bättre prestandapoäng och ökad användarnöjdhet.

Referenser
-----------------------

Google Developers. (u.å.). Mät webbprestanda med Google Lighthouse. Hämtad från https://developers.google.com/web/tools/lighthouse

Sidhastighet. PageSpeed Insights. Hämtad från https://pagespeed.web.dev/

Övrigt
-----------------------

Rapporten är skriven, analyserad och dokumenterad av Olof Jansson. En student som läser på distans i Göteborgsregionen.