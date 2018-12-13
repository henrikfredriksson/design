---
---

# Laddningstid

Denna rapport är en analys av laddningstiden av webbsidor hos tre svenska
lärosäten. Syftet med rapporten är att utvärdera laddningstiden och analysera
vad som är bra med webbsidorna, samt hitta förbättringspotential gällanade laddningstiden.

Rapporten har följande strukur. I avsnitt 2 så kommer jag beskriva hur mätdatan
togs fram och vilka verktyg som användes. I avsnitt 3 redogörs resultatet och
mätdatan från analysen. Rapporten avslutat med en diskussionsdel.

## Urval

Urvalsgruppen består av svenska högskolor och universitet. Webbsidorna har till
syfte att både presentera utbildningsutbud för att attrahera nya studenter och
för att informera om forskningsresultat.

Jag har valt att analysera tre lärosäten där jag har studerat. De tre lärosätena
är

- [Blekinge Tekniska Högskola](https://www.bth.se/)
- [Högskolan i Halmstad](https://www.hh.se/)
- [Linnéuniversitet](https://lnu.se/)

I fortsättning så kommer förtkortningarna BTH, LNU och HH användas för Blekinge
Tekniska Högskola, Högskolan i Halmstad respektive Linnèuniversitet.


Metod
-----------------------

Mätdatan är genererad med hjälp av verktyger [PageSpeed
Insights](https://developers.google.com/speed/pagespeed/insights/) och devtools
i webbläsaren Firefox. PageSpeed Insight poängsätter på en skala 0-100 där

 - 0-49 poäng är en långsam sida,
 - 50-89 poäng är en  medelsnabb sida och
 - 90-100 är en snabb sida.

Devtools mätningarna är genomförda tre gånger och
resultat som presenteras nedan är det aritmetiska medelvärdet av mätningarna.

Underlaget till mätvärderna i denna analys finns på [Google
Docs](https://docs.google.com/spreadsheets/d/1EZx6hexWobeChe4dgWRmDrk-pmzDjBnsDq9BZM3kHjg/edit?usp=sharing)

Som undersidor så har startsidan, studentportal och biblioteket sida valts för
undersökningen. 

Samtliga mätningar genomfördes den 11 december 2018, mellan 23.00-23.45.


## Resultat

### Blekinge Tekniska högskola [(www.bth.se)](https://www.bth.se)



[FIGURE src="image/bth_thumb.png?w=400" caption="Startsida av bth.se"]

BTH har även längst laddingstid av sidorna i testet.

|   | Mobile| Desktop |Laddningstid  (sekunder)  |Storlek (megabyte)  | Antal förfrågningar  |
|---|---:|---:|---:|---:|---:|
|[Startsida ](https://www.bth.se)    | 12 | 79 |15.75 | 11.29 |  136
|[Studentportal](https://studentportal.bth.se/page/hem)| 15 | 64 |14.36 | 3.71  |  37,7
|[Bibliotek](https://www.bth.se/bibliotek/)    | 18 | 94 |7.39  | 5.4   |  96

BTHs webbsida kan förbättra laddningstiden genom att välja bildformat med bättre
komprimerin och att genom att att ladda in JavaScript och CSS som inte syns i
ett senare skede.

### Linnéuniversitet [(www.lnu.se)](https://www.lnu.se)




[FIGURE src="image/lnu_thumb.png?w=400" caption="Startsida av lnu.se"]

|   |Mobile | Desktop | Laddningstid  (sekunder)  |Storlek (megabyte)  | Antal förfrågningar  |
|---|---:|---:|---:|---:|---:|
|[Startsida](https://lnu.se/)     |74 |  99  | 3.41  | 2.95 | 42.3
|[Studentportal](https://lnu.se/student/) |73 | 100  | 2     | 1.0  | 28.3
|[Bibliotek](https://lnu.se/ub/)    |30 |  96  | 8.38  | 7.11 | 55

Laddningstiden kan förkortas genom att använda mindre orginalstorlek på bilder än att
skala om dem och genom att skjuta upp inläsning av JavaScript och CSS.

### Högskolan i Halmstad [(www.hh.se)](https://www.hh.se)



[FIGURE src="image/hh_thumb.png?w=400" caption="Startsida av hh.se"]


|   |Mobile | Desktop | Laddningstid  (sekunder)  |Storlek (megabyte)  | Antal förfrågningar  |
|---|---:|---:|---:|---:|---:|
|[Startsida](https://www.hh.se/)     |41 |98   | 4.71 | 3.24  | 75.67
|[Studentportal](https://www.hh.se/arstudent/itstod/studentladok.65446689.html) |59 |100  | 2.74 | 1.84  | 48
|[Bibliotek](https://www.hh.se/bibliotek.243.html)    |29 | 88  | 4.73 | 2.27  | 56.78

Startsidan hh.se hämtar kontinuerligt bilder från ett Instagramflöde.
Laddningstiden är den tid det tar att ladda innan innan denna inläsning påbörjar.

HHs webbsida kan framförallt läsa in JavaScript och CSS mer effekt för att förkorta laddningstiden.

# Diskussion



Den förekommande kommentaren från PageSpeed Insight av testsidorna är att
laddningstiden kan förkortas ifall man skjuter upp inläsning alternativt asynkront läser
in JavaScript och CSS filer. Vissa JavaScript och CSS filer är nödvändiga för
att visa upp sidan innehåll.

Av testsidorna så är LNU vinnare, följt av HH, och däefter BTH.
Desktopvarianterna av LNUs sidor rankas som snabba av PageSpeed Insights, medans
2 av 3 tre sidor är medelsnabba av mobilvarianten.

Av HHs desktopsidor så rankas 2 av 3 sidor som snabba medans endast en
mobilvariant rankas som medelsnabb.

Av BTHs sidor så är det endast Biblotekssidan som rankas som snabb
(desktopvariant). Mobilstödet av BTHs sida är inte alls bra, då samtliga sidor
rankas som långamma.

PageSpeed Insights mätningar om laddningstid är ett mått på hur snabb en sida
är. Ett annat sätt att se på det är hur man som användare upplever
användbarheten hos sidan, d.v.s är sidan interaktiv, kan börja navigera runt, klicka
på länkar direkt när man besöker sidan. Man 

Ur denna aspekt så är ett tak på 2 sekunders
laddningstid acceptabelt ur mitt perspektiv. 

Sett ur användarperspektivet så klarar sig LNU och HH bra. Några av BTHs och HHs webbsidor har ibland
fenomenat att vypositionen ändras eftersom objekt blir synliga efter man har
börjat scrolla. När man klickar på BTHs Studentportalen så möts man dessutom av
nästintill blank med sida texten **Loading...**, vilket inte är någon trevlig
användarupplevelse.


Övrigt
-----------------------

Denna rapport är skriven Henrik Fredriksson som en del av kursmomenten kmom05 i
kursen Teknisk webbdesign och användbarhet.
