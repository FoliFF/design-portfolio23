---
Title: Load
Description: Rapport for colors
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
  <iframe width="300" height="200" src="https://docs.google.com/spreadsheets/d/e/2PACX-1vQv05aYqi2AwFz8-iwUuskk8EfDGk-dIY2xtLwQ0ESDB91TaYYzEQClTvIzqH7hVvHYT96y5WLY6sEH/pubhtml" title="Web result" frameborder="0" allowfullscreen></iframe>
</div>


#### Chalmers Tekniska Högskola
•	Mobil: PageSpeed Insights ger betyget 73 för prestanda med viktiga måttvärden som First Contentful Paint på 1,4 sekunder och Time to Interactive på 5,6 sekunder.
•	Desktop: Prestationsbetyget är 94 med en First Contentful Paint på 0,5 sekunder och en snabb Time to Interactive på 1,5 sekunder.
•	DevTools mätningar visade en genomsnittlig laddningstid på 603 ms med 32 resurser som laddas.
#### Blekinge Tekniska Högskola
•	Mobil: PageSpeed Insights visar 91 i prestanda med en First Contentful Paint på 0,7 sekunder.
•	Desktop: Betyget för prestanda är 94 med en First Contentful Paint på 1,5 sekunder.
•	DevTools: Genomsnittlig laddningstid är 564 ms för sidan med 42 resurser som laddas.
#### Skatteverket
•	Mobil: Lågt prestandabetyg på 52 från PageSpeed Insights och en First Contentful Paint på 6,3 sekunder.
•	Desktop: Prestationsbetyget förbättras till 72 med en First Contentful Paint på 1,8 sekunder.
•	DevTools: Sidan laddas i genomsnitt på 547 ms med totalt 40 resurser.


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