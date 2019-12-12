Laddningstid
=======================

Denna uppgift handlar om att välja ut ett antal olika webbplatser och testa dem
för att mäta och utvärdera deras laddtid samt innehåll.

Urval
-----------------------

Jag har valt att analysera mmsports.se, monkeysports.se samt intersport.se. Det är
tre sidor som säljer produkter som jag är intresserad av samt att jag brukar handla från dessa sidor. Därför är jag intresserad av hur dom presterar i mätningarna samt om det finns förbättringspotential.

Metod
-----------------------

Jag kommer utföra denna analys med hjälp av Google PageSpeed. Detta verktyg
mäter sidans laddtid samt analyserar och ger rekommendationer på förbättringar.
Webbläsaren som används är Google Chrome. Jag kommer även mäta antal
resurser, sidans laddtid samt storlek med hjälp av Chrome devtools. Cache kommer
vara avstängt under mätningarna. Jag kommer att kolla startsidorna, Rea/kampanjsidorna samt en enskild produkts sida.

Resultat
-----------------------
####mmsports.se
[FIGURE src=image/mmsports.png?w=1000]

mmsports får toppbetyg på desktop samt höga betyg på mobil. Potentiella förbättringar
skulle för mobil kunna vara att minska på DOM-trädet samt att minska arbetsbelastningen på modertråden. Det verkar även finnas möjlighet till att ta bort oanvänd CSS. För desktop är största boven DOM-trädet. Storleken på sidorna ligger mellan 0,7-1,1 MB och laddtiden går från ca 0,5s till just över en sekund

####intersport.se
[FIGURE src=image/intersport.png?w=1000]

Intersport får rätt bra betyg på desktopsidan medans mobilsidan får ett dåligt betyg.
Förbättringar på mobilsidan kan göras med hjälp utav modernare bildformat, skjuta upp inläsning av
bilder som inte visas på sidan, minska körningstiden för JavaScript samt att minska
belastningen på modertråden. För desktopsidan skulle DOM-träden kunna minskas samt
att man bör se till att all text förblir synlig medans webbteckensnitten läses in. Storleken på sidorna startar på just under en MB och den största mättes till 1,9 MB. Laddtiderna låg mellan 1-1,24s.

####monkeysports.se
[FIGURE src=image/monkeysports.png?w=1000]

monkeysports får extremt dåligt betyg på sin mobilsida samt dåligt på desktop. Det finns
stor förbättringspotential på både mobil och desktop genom att skicka bilder i ett modernare format, ta bort resurser som blockerar renderingen samt att koda bilderna mer effektivt. Mätningens största webbplats som låg mellan 2,2 och 5,3 MB. Laddtider på 1-1,22s.

Länk till kalkylark med rådata [här](https://docs.google.com/spreadsheets/d/1zgexF0SQgKTLaxXXf-rg3cgGS1naFEHIbrISTRCpVVw/edit?usp=sharing).


Analys
-----------------------

Sammanfattningsvis så är det tre olika webbplatser som lägger sig i tre olika betygsklasser. Alla är inom samma branch (sport/försäljning) och alla är tre nationella och stora aktörer inom sitt område. Det är förvånande att så stora aktörer som monkeysports och intersport får så låga betyg. Speciellt monkeysports som mer eller mindre får ett horribelt resultat.
Det finns ju inte jättemycket förbättringspotential hos mmsports eftersom dom får toppbetyg men gemensamt med både intersport och monkeysports är att man skulle kunna minska storleken på DOM-trädet. Alla tre sidor ligger över rekommendationen på 1500 DOM-element. Monkeysports och Intersport har dock ett antal förbättringspunkter gemensamt. Båda webbplatserna verkar ha bilder i ett äldre webbformat, hög arbetsbelastning på modertråden samt resurser som blockerar renderingen. Bilder är ju ett av de viktigaste delarna när det kommer till webbplatser som har försäljning som huvudsyfte så det
borde ligga i företagens intresse att se till så man visar bilderna på ett effektivt sätt. Studier har visat att sidors laddtid har en direkt påverkar på försäljningen.

En rangordning av dessa webbplatser är rätt enkel. Mmsports är en klar vinnare i både betyg av PageSpeed samt i laddtider. Intersport får bra betyg på sin desktopwebbplats och trots låga betyg för mobilsidan så är dom ändå klart före Monkeysports. Monkeysports får minimalt betyg på mobilsidan och dåliga betyg på desktop vilket gör dom till testets klart sämsta webbplats. Dock är laddtiderna i klass med Intersport.

Jag skulle säga att en snabb webbplats har en laddtid på max en sekund vilket Mmsports klarar. En långsam webbplats tycker jag nog tar uppemot 2 sekunder på sig, vilket ingen webbplats är i närheten av i detta test. Rent generellt känns dock både Intersport och Monkeysports ganska långsamma i navigeringen. Mmsports verkar inte ha några problem med snabbheten.

Referenser
-----------------------
[mmsports.se](https://www.mmsports.se/home.php)

[intersport.se](https://www.intersport.se/)

[monkeysports.se](https://www.monkeysports.se/)

[https://developers.google.com/web/fundamentals/performance/why-performance-matters/](https://developers.google.com/web/fundamentals/performance/why-performance-matters/)

Övrigt
-----------------------

Rapporten är skriven av Gustav Berg.
