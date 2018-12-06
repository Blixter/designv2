Utvärdering på laddningstid
=======================

Jag har valt tre olika webbplatser för att testa hur fort de laddas och vad de kan göra för att förbättra laddningstiden.

Urval
-----------------------

Jag valde tre stora bankers webbplatser. Jag tycker att det kan vara intressant att fortsätta med samma webbplatser som senast, men istället jämföra deras laddningstid och användarbarhet. För att se vilka resultat jag får fram här istället.
Dessa sidor har jag valt: [Nordea](https://www.nordea.se/), [Swedbank](https://www.swedbank.se/) och [Icabanken](https://www.icabanken.se/).




Metod
-----------------------
Jag har använt mig av [Googles PageSpeed](https://developers.google.com/speed/pagespeed/insights/). Det är ett verktyg som kan analysera innehållet på hemsidor och poängsätter dem från 0 till 100, samt ger råd på hur respektive webbplats kan förbättras. Jag har även använt mig av Devtools och gått in på nätverk, där jag har kollat laddningstiden på de olika webbplatserna, kollat hur många resurser man går igenom vid laddningstillfället, samt sidornas storlekar.



Resultat
-----------------------

######Nordea######
[FIGURE src="image/nordeaklipp.jpg?width=900&q=90" caption="Nordeas Webbplats."]

| Nordea | Resultat |
|-----|--------|--------|
| PageSpeed Mobil| 71 |
| PageSpeed Dator| 100 |
| Laddningstid (snittid)| 1.71 sekunder |
| Antal resurser | 28 |
| Sidans storlek | 930 KB |

######Swedbank######
[FIGURE src="image/swedbankklipp.jpg?width=900&q=90" caption="Swedbanks Webbplats."]

| Swedbank | Resultat |
|-----|--------|--------|
| PageSpeed Mobil| 11 |
| PageSpeed Dator| 94 |
| Laddningstid (snittid)| 3.05 sekunder |
| Antal resurser | 55 |
| Sidans storlek | 7 MB |


######ICABanken######
[FIGURE src="image/icabankklipp.jpg?width=900&q=90" caption="ICABankens Webbplats."]

| ICABanken | Resultat |
|-----|--------|--------|
| PageSpeed Mobil| 77 |
| PageSpeed Dator| 98 |
| Laddningstid (snittid) | 2.52 sekunder |
| Antal resurser | 48 |
| Sidans storlek | 1.2 MB |

[Google Kalkylark där jag dokumenterade mina test.](https://docs.google.com/spreadsheets/d/1KS-dI8onB-LaTPFcgE4HqWIdDLgSy68OhORURXwTfxo/edit#gid=0)

Analys
-----------------------
Swedbank behöver helt klart förbättra sin sida. De kan ändra sina bildformat till ett format som ger bättre komprimering. De använder JPEG och PGN, och enligt PageSpeed är det bättre att välja andra bildformat som t.ex. WebP. Framför allt så behöver Swedbank använda bilder med en mindre storlek på mobilen, just nu har Swedbank en bild som är 4 599 KB stor, vilket är är oeherhört stort för att ladda, och gör att laddningstiden blir långsam. Bilden har en upplösning på 2000 x 1201 pixlar, även på mobilen. En webbplats bör aldrig använda bilder som är större än vad som visas på användarens skärm, det är bara onödig data som behöver laddas ner.

Nordea använder sig av bättre bildstorlekar. Även här tipsar PageSpeed om att använda modernare bildformat så som JPEG 2000, JPEG XR och WebP. De kan även skjuta upp sådant som inte visas på skärmen, så det läses in med så kallad lat inläsning. Det är alltså möjligt att bara läsa in 'above-the-fold'-bilderna vid första inläsningen. För att sedan läsa in de resterande bilderna vid ett senare tillfälle, t.ex. när användaren börjar skrolla ner. 

På Icabankens webbplats tipsar PageSpeed återigen om bildformaten. Jag tror dock att det är vanligt att man använder sig av jpeg-format, och att Google gärna vill pusha för att man skall gå över till deras egna bildformat WebP. Det som även IcaBanken kan göra är att skjuta upp bilder som inte visas på skärmen vid första inladdningen.

Om jag skulle ranka dessa sidor så anser jag att Nordea har den bäst optimerade webbplatsen, den har en storlek under 1 MB och inte alls för många resurser. Nordeas laddningstid på 1.71 sekunder är en snabb laddningstid. På andra plats hamnar Icabanken, fler resurer att gå igenom än Nordea och lite större sidstorlek. Men ändå helt godkänd laddningstid. Swedbank däremot bör göra något åt deras storlek på 7 MB, därav den långa laddningstiden. Swedbank blir alltså sist i mitt test.

Jag personligen anser inte att någon av dessa sidor känns långsam, det är ändå rätt tunga sidor med mycket data, många bilder, massvis av länkar och information. Så jag anser att alla har en godkänd laddningstid. Om jag skulle välja en gräns för absolut laddningstid, så blir en sida för långsam om laddningstiden är över 5 sekunder, ligger den på runt 2 sekunder så klassar jag det som en snabb webbplats.


Referenser
-----------------------

Webbplatser:<br>
[Moz om Page Speed.](https://moz.com/learn/seo/page-speed)<br>
[Google om laddning av bilder utanför skärmen.](https://developers.google.com/web/tools/lighthouse/audits/offscreen-images)<br>
[Google om laddning av förstora bilder.](https://developers.google.com/web/tools/lighthouse/audits/oversized-images)<br>

Kurslitteratur:<br>
Titel:	The Principles of Beautiful Web Design<br>
Utgiven, revision, antal sidor:	2014, Third edition, 220s<br>
Författare:	Jason Beaird<br>
Förlag:	SITEPOINT<br>
ISBN:	9780992279448

Övrigt
-----------------------

Utvärderingen gjord av Robin Blixter.
