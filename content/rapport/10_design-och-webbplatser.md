Analys design och webbplatser
=======================
Jag har fått i uppdrag av organisationen "Valfrihet" att göra en analys inom design och webbplatser.
Jag kommer därför att undersöka webbplatsers laddningstider, storlek och innehåll. Utöver detta kommer jag
även att ge förslag på förbättringar utifrån analysens resultat.

Urval
-----------------------
Jag har valt att analysera startsidorna för de fem Nyhetssajter som kom med på idg.se top100 webbplatser 2019. Aftonbladet, DN, Expressen,
Omni samt SVT Nyheter. Anledningen till detta urval är att det är hård konkurrens i nyhetsbranchen och jag tror det är
viktigt med en bra optimerad webbplats för att kunna locka så många besökare som möjligt. Upplevs hemsidan långsam så
tror jag att de flesta söker sig vidare till en annan webbplats.

Metod
-----------------------
Med hjälp utav Google PageSpeed kommer jag att utvärdera och analysera webbsidornas prestanda för både desktop och
mobilsidorna. Webbläsaren jag kommer använda mig utav är Google Chrome och jag kommer att mäta sidornas laddtid, storlek och antal resurser.
Google PageSpeed ger förslag på förbättringar för att öka betyget vilket jag kommer att lista i resultatet. Jag kommer även använda mig
utav Chrome devtools för att mäta sidornas storlek, antal resurser samt laddtid.

Resultat
-----------------------
Länk till excelark med resulten finns [här.](https://docs.google.com/spreadsheets/d/1WlFVJcWhjrVk-EzB-PYpFR9UXg-DyoU-bH6J7Lk_aCA/edit?usp=sharing)
#####Aftonbladet
PageSpeed betyg för desktop: 67/100, mobil: 36/100.
Desktopsidan är 1,1 MB stor, laddar 78 resurser och har en loadtime på 1,5s.

För desktop så finns det en hel del förbättringspotential om dom skulle skicka bilderna i modernare bildformat, ta bort oanvänd CSS samt ta bort resurser som blockerar renderingen. Cirka 0,6s laddtid hade kunnat skalats av med hjälp utav detta. Övriga förbättringsområden skulle kunna vara att minska storleken på DOM-trädet samt att använda sig av en effektivare cachelagringspolicy.

Mobilsidan har liknande förbättringsområden med tillägg av att inläsningen av bilder som inte visas på skärmen skulle kunna skjutas upp och att man skulle kunna koda bilder mer effektivt.
En begränsning av tredjepartskod och en minskad körningstid av JavaScript hade också gett en positiv effekt för sidans laddtid.


#####DN
PageSpeed betyg för desktop: 94/100, mobil: 78/100.
Desktopsidan är 902 KB stor, laddar 63 resurser och har en loadtime på 513ms.

Desktopsidan är väldigt bra optimerad och får riktigt högt betyg av PageSpeed. Den största
förbättringen skulle vara att skicka bilderna i ett modernare format men man skulle även kunna
försöka att minska på DOM-trädet en aning samt att använda en lite effektivare cachelagringspolicy.

Mobilsidan får relativt bra betyg men här finns det utrymme för en del förbättringar. Minifiering
av JavaScript, användning av rätt storlek på bilder samt skjuta upp inläsningen av bilder som
inte visas på skärmen hade varit att rekommendera. PageSpeed anser också att det bör gå att
minska svarstiderna från servern.

######Expressen
PageSpeed betyg för desktop: 79/100, mobil: 89/100.
Desktopsidan är 1,7 MB stor, laddar 79 resurser och har en loadtime på 647ms.

Desktopsidan får rätt bra betyg. Detta hade kunnat förbättras ytterligare genom att skjuta upp
inläsningen av bilder som inte visas på skärmen, minska svarstiderna från servern en minskning
utav DOM-trädet. Även en viss effektivisering av cachelagringspolicyn hade gett effekt.

Mobilsidan får väldigt bra betyg och här finns det inga superstora områden att förbättra. En minskan av
tredjepartskod samt en  minskad arbetsbelastning på modertråden hade dock varit optimalt.

#####Omni
PageSpeed betyg för desktop: 76/100, mobil: 55/100.
Desktopsidan är 1,8 MB stor, laddar 66 resurser och har en loadtime på 1,74s.

Desktopsidan får ett medelhögt betyg och det finns ett antal punkter att förbättra den på. Uppsjuktning av inläsningen för
bilder som inte visas på skärmen, skicka bilder i modernare bildformat samt att använda bilderna i rätt storlek hade varit
en bra början. Minskad belastning på modertråden, minskad körningstid av JavaScript en effektivare cachelagringspolicy
skulle vara optimalt.

Mobilsidan har liknande brister fast i ännu större utsträckning. PageSpeed ger en uppskattad tidsbesparing på drygt 13 sekunder
om alla bildrelaterade optimeringar utförs.

#####SVT Nyheter
PageSpeed betyg för desktop: 83/100, mobil: 37/100.
Desktopsidan är 1,5 MB stor, laddar 117 resurser och har en loadtime på 937ms.

Ett bra betyg på desktopsidan ger inte mycket förbättringsområden men dom största är minskning av svarstiderna från servern,
uppsjuktning av inläsningen för bilder som inte visas på skärmen och borttagning av resurser som blockerar renderingen.
DOM-trädet skulle även kunna minskas för optimal prestanda.

Mobilsidan lämnar dock en hel del att önska. Samma förbättringsområden som desktopsidan men oanvänd CSS skulle behövas tas bort.
Minskad arbetsbelastning på modertråden, mindre DOM-träd samt minskad körningstid för JavaScript hade också varit välbehövligt.

Analys
-----------------------
Snittbetyget för desktopsidorna hamnar på 79,8 och för mobil ligger det på 59. Betyg mellan 50 och 89 kallar Google PageSpeed för "average"
eller på svenska, medel. Då denna analys innefattar de några av de största nyhetssajterna i landet så är det i mitt tyckte ett ganska dåligt
betyg. En punkt som 3 utav 5 webbplatser får kritik för är att dom skulle kunna använda sig av ett modernare bildformat. Det tycker jag
är anmärkningsvärt eftersom att i princip alla nyheter som publiceras idag innehåller minst en bild. Alla webbplatser utom Omnis fick
rekommendationen att minska på DOM-trädet. Såhär beskriver LightHouse rekommendationerna gällande DOM-träd:
>"Webbutvecklare rekommenderar att sidor innehåller mindre än 1500 DOM-element. Det bästa är ett träddjup med mindre än 32 element och högst 60 underordnade/överordnade element. En stor DOM kan öka minnesförbrukningen, förlänga formatberäkningarna och producera kostsamma flödesuppdateringar för layouten."

En annan stor förbättringspunkt hos alla fem webbplatser är att minska belastningen på modertråden. Detta görs enligt LighHouse enklast genom att minska storleken på
JavaScript-resurserna som skickas. Något som förvånade mig var att Aftonbladet och SVT rent ut sagt fick riktigt dåliga betyg på sina mobilsidor.
Även Omni fick ett lågt betyg. Enligt rapporten [Svenskarna och internet 2019](https://svenskarnaochinternet.se/app/uploads/2019/10/svenskarna-och-internet-2019-a4.pdf) så använder 90% av befolkningen internet i mobilen och 61% internet i surplatta. På daglig basis så använder 87% av internetanvändarna
mobilen jämfört med att 67% använder datorn. En förklaring till detta kan vara att Nyhetssajterna ofta har en egen app, och dom kanske förväntar sig att majoriteten
av användarna kommer att använda sig utav den istället för mobilsidan. Ytterligare en intressant undersökning i denna rapport är att 60% av internetanvändarna
uppger att deras tid används meningsfullt vid användandet av respektive app/e-tjänst i kategorin "Nyhetsappar". Detta var toppnoteringen i undersökningen. Så även fast min analys visar
på att mobilsidorna får relativt dåliga betyg så verkar internetanvändarna nöjda.

Aftonbladet och Omni stack ut med laddtider som var i det längsta laget (1,5 respektive 1,74s). Just laddtiden har visat sig vara väldigt viktig när
det kommer till att få användarna att stanna kvar på webbplatsen. enligt en [rapport](https://www.thinkwithgoogle.com/marketing-resources/data-measurement/mobile-page-speed-new-industry-benchmarks/) släppt utav Google i februari 2018 så ökar sannolikheten för att användaren lämnar webbplatsen med 32% när laddtiden går från 1 sekund till 3. Går den från 1s till 5 så ökar sannolikheten med 90%. Nu var ingen av de 5 webbplatserna i denna analys i närheten av
sådana laddtider men det visar på hur viktigt det är med korta laddtider för att tillfredsställa användarna. Nu börjar datan i Googles rapport bli gammal
och det skulle inte förvåna mig om kraven hos användarna gällande laddtid blivit ännu högre 2020 kontra 2018. Snittladdtiden på de 5 webbplatser i denna
analys blev just över 1 sekund vilket får anses godkänt i mitt tycke.

Sammanfattningsvis så blev snittbetyget för dessa webbplatser "medel" enligt Google PageSpeed och jag har tagit upp några av de största problemområdena
som dessa webbplatser bör kunna förbättra. Jag hade förväntat mig höga betyg då dessa är några av Sveriges ledande nyhetssajter och en del forskning
tyder på att webbplatsers prestanda har en stor betydelse för användarnas benägenhet att stanna.



Referenser
-----------------------
[Svenskarna och internet 2019](https://svenskarnaochinternet.se/app/uploads/2019/10/svenskarna-och-internet-2019-a4.pdf)

[Think with Google](https://www.thinkwithgoogle.com/marketing-resources/data-measurement/mobile-page-speed-new-industry-benchmarks/)

[Aftonbladet](https://www.aftonbladet.se/)

[DN](https://www.dn.se/)

[Expressen](https://www.expressen.se/)

[Omni](https://omni.se/)

[SVT](https://www.svt.se/)


Övrigt
-----------------------

Rapporten är skriven av Gustav Berg.
