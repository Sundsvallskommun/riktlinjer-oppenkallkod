# Riktlinjer för hanteringen av öppen källkod

Dessa riktlinjer är i första hand framtagna för att gälla API-teamet inom Sundsvalls Kommun, men hoppas kunna utvidgas till att gälla större delar av Sundsvalls Kommuns verksamhet på sikt.

## Bakgrund

I takt med att Sundsvalls Kommun ökar digitaliseringstakten och sitt användande av öppen källkod, har det uppstått ett behov av att sammanställa en riktlinje för hur exempelvis anskaffning, utveckling och publicering av tjänster baserade på just öppen källkod skall gå till.

Att publicera en sådan riklinje öppet känns som ett naturligt steg och i vårt arbete har vi inspirerats av tidigare publiceringar från bland andra Myndigheten för Digital Förvaltning (DIGG) och [Försäkringskassan](https://github.com/forsakringskassan/riktlinje-oppenkallkod).

## Skapande och publicering av öppen källkod

### Syftet med publicering

* Underlätta utveckling 
* Främja samverkan i ett ekosystem
* Uppmuntra till återanvändning

### Checklista inför första publicering

Följande lista är en anpassning av de punkter som Försäkringskassan tar upp i sin riktlinje. Vi anser att de utgör en bra utgångspunkt även för vår verksamhet.

* Innehållet ska utifrån gällande informationsklassningsmodell och säkerhetsskydd vara lämpligt för publicering.
* Källkod skall vara parametriserad och får inte innehålla hårdkodade konfigurationsparametrar.
* Källkoden får inte omfattas av en licensmodell som omöjliggör publicering.
* Källkodens härkomst skall vara känd
* Om tredjepartsprogramvara används i källkodsform måste licensformerna vara kompatibla och ingå till fullo eller i enlighet med tredje parts krav.
* Kvaliteten på publicerat innehåll ska vara hög och inte innehålla irrelevant information.
* Publicerat material får inte utsätta kommunen för ökad risk eller på annat sätt påverka kommunens anseende negativt.
* Licensformen ska vara bestämd och vara godkänd av Open Source Initiative.
* Säkerhetsbedömning av källkod ska göras och åtgärder ska vidtas för att säkra kvalitet.

### Hur publicerar vi

Sundsvalls Kommun har valt GitHub som den plats där vi publicerar öppen källkod. För de tjänster som kan anses lämpliga för publicering, enligt checklistan ovan, gäller att den huvudsakliga utvecklingen skall ske mot ett publikt kodarkiv (repository) under vår organisation på [https://github.com/sundsvallskommun]. Anledningen till denna strategi är att öka möjligheten till samverkan och stimulerande av livskraftiga ekosystem. Genom att inte låsa in utvecklingen utom räckhåll för externa parter, ökar vi möjligheten för dessa att bidra till och dra nytta av det arbete vi gör.

För publicering har två huvudsakliga licensformer valts ut för vårt arbete.

De tjänster som API-teamet levererar skall i första hand publiceras under licensformen MIT för att tillåta ett fritt återanvändande och möjliggöra för delaktighet från en större andel potentiella aktörer.

Tjänster som å andra sidan kan anses utgöra en del av en större sammanhängande plattform, skall däremot i första hand publiceras under licensformen AGPL-3 som verkar mer skyddande för kommunens investeringar i öppen programvara.

### Checklista inför löpande uppdatering

För att säkerställa bibehållen kvalitet gäller följande:
* Kod är byggd enligt gällande standard med en kvalitet som tål öppenhet
* Kod och tester är granskade av annan teammedlem
* Feature-brancher stängda och allt mergat till main
* Att koden levererar önskad funktion skall vara avstämd med beställare
* Sandbox skall vara uppdaterad
* Design- och API-dokumentation skall vara uppdaterad

### Hantering av återkoppling från andra

Rapporterade buggar och initierade pull requests prioriteras i respektive utvecklingsteams löpande arbete.

## Vidmakthållande av riktlinjen

Löpande förbättringar samt kvalitetskontroll av denna riktlinje sköts som en linjeaktivitet inom avdelningen Digitalisering & Innovation på Sundsvalls kommun.
