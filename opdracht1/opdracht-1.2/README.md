# Browser technologies
## Opdracht 1.2 - Fork je OBA
[Link naar de repository](https://github.com/baskager/ADRmeta)

## Pas Progressive enhancement toe op je OBA Web App
Om progressive enhancement toe te passen zou ik de data server-side moeten renderen. Om dit om te bouwen is te veel werk voor de scope van deze opdracht.

## Check je OBA Web App op de 8 features uit opdracht 1.1 en verbeter de code waar mogelijk

#### Afbeeldingen
Gezien de webapp portretten vergelijkt is het bijna onmogelijk om de personen te vergelijken. Men kan alleen de tekst gebruiken om te controleren of eenzelfde persoon op een portret staat.

Het tonen van afbeeldingen is een must-have voor deze app gezien deze zo visueel ingesteld is.
![Test zonder afbeeldingen](http://kager.io/uploads/minor/browser-technologies/no-images.png)

#### Custom fonts
Het font veranderd iets maar de app blijft zichtbaar en bruikbaar
![Test zonder custom fonts](http://kager.io/uploads/minor/browser-technologies/no-custom-fonts.png)

#### Javascript (volledig)
De gehele app werkt niet zonder javascript. Net als afbeeldingen is javascript een must-have voor het laten werken van deze webapp. Om dit te fixen zou de data server-side gerenderd moeten worden. Dat is veel werk en uit de scope van de werkzaamheden voor deze week.
![Test zonder javascript](http://kager.io/uploads/minor/browser-technologies/no-javascript.png)

#### Kleurenblindheid
![Kleurenblindheid test](http://kager.io/uploads/minor/browser-technologies/color-blind.png)
De webapp is goed zichtbaar en alle features van de app zijn nog steeds bruikbaar in verschillende vormen van kleurenblindheid.

#### Breedband internet
De app laadt alle afbeeldingen in de collectie in een keer. Dit zorgt er voor dat de app op een breedband connectie erg lang op zich laat wachten. Hier zijn zeker verbeteringen in te maken.

- De DOM werdt in 12.60 seconden geladen met 128 kb/s
- De gehele app en alle portretten waren in 8.7 minuten geladen


De app kan geoptimaliseerd worden op breedband internet door een beperkt aantal portretten per request op te halen. Het laden van overige portretten zou doormiddel van scrollen kunnen.

#### Cookies
De app maakt geen gebruik van cookies en wordt niet gehinderd door het uitzetten van deze functionaliteit. Hier zijn dus geen optimalisaties mogelijk.

#### LocalStorage
In de PDF van opdracht 1.1 staat uitgebreid beschreven wat er gebeurd als localstorage uitgezet wordt. De app functioneert niet naar verwachten als LocalStorage niet beschikbaar is.

Mijn oplossing hiervoor is om een 'storage' klasse te schrijven die terugvalt naar een mogelijke opslagmethode als LocalStorage niet beschikbaar zijn.
#### Muis/Trackpad
De volledige collectie en alle pagina's zijn middels tabs te navigeren. Bij elke tab komt het gefocusde portet naar voren en krijgt deze extra schaduw.

De app is zonder muis of trackpad te gebruiken

## Test je OBA Web App in het device lab
Op de meeste devices werkt de app niet omdat EcmaScript 6 modules en classes gebruikt worden. Een oplossing voor dit probleem is om de javascript naar ES5 te compilen middels babel.

Op de LG nexus werkte de webapp omdat deze mobiel standaard wordt geleverd met Google Chrome als browser. Deze browser biedt ondersteuning voor de gebruikte ES6 code. De portretten zijn goed zichtbaar en zijn aan te klikken. Er zijn wel wat verbeteringen mogelijk wat betreft de layout.

![LG Nexus app test](http://kager.io/uploads/minor/browser-technologies/lg-nexus-test.jpg)

Ook kwam ik achter een kleine probleem met de responsive grid, dat probleem is in [deze issue](https://github.com/baskager/ADRmeta/issues/3) gefixed :).

## Laat je OBA Web App voorlezen door een screenreader
Alle items zijn middels tabs te navigeren en worden vervolgens voorgelezen. In de detailpagina gebeurd dit ook.

**Mogelijke verbeteringen:**
- In de detailpagina wordt de metadata zoals leeftijd niet voorgelezen, dit zou verbeterd kunnen worden.
- Er wordt niet voorgelezen dat het om een afbeelding/portret gaat


![Kleurenblindheid test](http://kager.io/uploads/minor/browser-technologies/screenreader.png)

## Gebruik onderstaande artikelen om je code te optimaliseren
- https://24ways.org/2015/the-accessibility-mindset/
- https://www.smashingmagazine.com/2015/02/bbc-iplayer-accessibility-case-study/

**Mogelijke verbeterpunten na het lezen van de artikelen:**
- De titel van een portret wordt twee keer genoemd omdat de titel ook in de 'alt' tag van de afbeelding is verwerkt
- De app kan beter uitgelegd worden voor screenreader gebruikers, de uitleg bovenaan de pagina wordt niet voorgelezen door de screenreader
