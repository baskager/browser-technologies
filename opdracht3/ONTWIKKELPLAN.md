# Ontwikkelplan opdracht 3
De opdracht die ik heb gekozen voor deze week is:

    "Ik wil tegen de helpdesk kunnen klagen over een iframe-dat-het-niet-doet, en direct antwoord krijgen."

### Wensen van de klant
- Gebruik de Pattern Primer van de Voorhoede om de use case te ontwerpen. (bepaal de core functionaliteit, acceptable en de enjoyable laag)
- Een beschrijving van de core functionality
- Een beschrijving van de Features en welke browsers deze features ondersteunen
- Een beschrijving van de accessibility features die zijn onderzocht
- De demo is opgebouwd uit drie lagen, volgens het principe van progressive enhancement
- De user experience van de demo is pleasureable
    - De leesbaarheidsregels zijn toegepast, contrast en kleuren kloppen
    - Het heeft een pleasureable interface met gebruikmaking van affordance en feedback op de interactieve elementen
- Student kan uitleggen wat progressive enhancement en feature detectie is en hoe dit toe te passen is in web development.

### Core functionality
De core functionaliteit is dat de klant zijn klacht kan indienen op de website, zelfs als javascript uit staat. Dit wil ik bereiken door de aanvraag uit het formulier server-side te ontvangen.

### Features en browserondersteuning
Met progressive enhancement wil ik dit vervolgens gebruiksvriendelijker maken doormiddel van ajax requests, de klant krijgt dan een bevestiging op het scherm te zien op het moment dat de klacht succesvol verzonden is.

Een optionele feature wordt dat scheldwoorden opgemerkt worden. Deze schulden voeden in de achtergrond een soort 'woede' meter waardoor de interface roder en intenser wordt. Denk aan vlammen en grote teksten (vergelijkbaar met mood lighting), hierdoor krijgt de klant het gevoel dat hij lekker zijn woede kwijt kan.

Deze scheldwoorden verdwijnen uiteindelijk uit de klacht waardoor de klantenservice medewerker niet beledigt wordt. De klantenservice medewerker krijgt wel een indicatie van de boosheid van de klant te zien (de eerder besproken woedemeter).

Gezien het klachtenformulier gebruik maakt van basale HTML-elementen verwacht ik dat de site ook op simpelere en oudere versies van browsers werkt. De GUI zal dan wel minder pleasureable zijn. Het kan voor gebruikers van oudere of simpelere browsers zo zijn dat bepaalde "enhancements" niet (optimaal) zullen werken

##### Features in een notendop
- De klant kan een klacht indienen in de meest basale (html only) versie va de website
- De klant kan een klacht indienen in de enhanced versie van de website. Dit is een 'pleasureable' interface die gebruik maakt van AJAX requests.
- (OPTIONEEL) De klant mag er op los schelden waardoor op de achtergrond een 'woedescore' berekent wordt. De interface wordt dan vanzel 'bozer' in zijn stijl (een soort moodlighting).



### Accessibility
- De site moet voorgelezen kunnen worden door een screenreader
- De site moet zonder muis of trackpad te gebruiken zijn (keyboard-input)
- Het contrast en de kleuren moeten zo zijn dat de website leesbaar is voor slechtzienden en kleurblinden
- Proper gebruik van headings conform webstandaarden
- Toepasselijke alt tags voor images
- Links en navigatie uniek en goed beschreven
- Proper en standaardconform gebruik van HYML formulier elementen
- Dynamische content duidelijk voor screen readers. Licht een screen reader in zodra het formulier succesvol verstuurd is.
- (Optioneel) Licht de gebruiker in over de 'woede meter' status



### Bronvermelding
[Berkeley Web Access - Top 10 Tips for Making Your Website Accessible](https://webaccess.berkeley.edu/resources/tips/web-accessibility)

[Berkeley Web Access - Tools for finding issues (accessibility)](https://webaccess.berkeley.edu/evaluating/self-assessment/tools)

[Opdracht 3 - Beoordelingscriteria](https://docs.google.com/presentation/d/1wlGm2j_l_wbrvgkqo5XEdQG9Qn0auPEnQmGU6pqMUOQ/edit#slide=id.g120910d6b4_0_7)
