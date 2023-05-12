## Velkommen til kodeoppgave 1 i NAV FORS!


## Kan du slå Marit i Blackjack?


## Om oppgaven
* Du kan benytte hvilket programmeringsspråk du vil
* Når du møter til intervju så vil vi at du kan demonstrere kjørbar kode.
* Oppgaven skal være dokumentert på en måte som gjør at vi forstår hva som skal til for å kjøre den.
* Besvarelse med tester er ikke et krav, men vil gi plusspoeng.
* Hvis du ønsker å vise din front-end-kompetanse, kan du gjerne lage en front-end, men det er ikke et krav.


## Regler (1)
* To spillere, du og Marit, skal spille mot hverandre!
* Hver spiller tar to kort hver fra toppen av en tilfeldig stokket kortstokk. 
    * Endpointet for dette finner du her: https://blackjack.ekstern.dev.nav.no/shuffle
* Du tar de to første kortene, Marit tar de to neste
* Regn ut den samlede poengsummen til hver spiller
    * Nummererte kort har poeng som angitt på kortet 
    * Knekt (J), Dronning (Q) og Konge (K) teller som 10 poeng
    * Ess (A) teller som 11 poeng
* Regn ut om en av spillerene har 21 poeng  - Blackjack - med deres initielle kort, og dermed vinner runden.


## Regler (2)
* Hvis ingen har 21 poeng, skal spillerne trekke kort fra toppen av kortstokken
    * Du skal stoppe å trekke kort når poengsummen blir 17 eller høyere
    * Du taper spillet hvis poengsummen er høyere enn 21
    * Når du har stoppet å trekke kort, begynner Marit å trekke kort
    * Marit slutter å trekke kort når poengsummen hennes er høyere enn din poengsum
    * Marit taper spillet dersom poengsummen er høyere enn 21
* Skriv ut hvem  som vinner spillet
* Skriv ut poengsum og kortene til hver spiller ved spillets slutt. Et kort angis ved å konkatenere `suit` og `value`:
    * `suit` -> [`H`|`D`|`S`|`C`]
    * `value` -> [`2`|`3`|`4`|`5`|`6`|`7`|`8`|`9`|`10`|`J`|`Q`|`K`|`A`]
* Eksempel på output:
        Vinner: Truls
                                  
        Marit | 27 | S7,S10,CJ
        Truls  | 19 | D2,H2,C6,H9


## Om kortstokken
* Kortstokken finnes på https://blackjack.ekstern.dev.nav.no/shuffle
* Formatet på kortstokken er en JSON-array med 52 elementer
* Hvert element er et objekt med  egenskapene `suit` og `value`
    * `suit` -> [`HEARTS`|`DIAMONDS`|`SPADES`|`CLUBS`]
    * `value` -> [`2`|`3`|`4`|`5`|`6`|`7`|`8`|`9`|`10`|`J`|`Q`|`K`|`A`]
* Eksempel:            
            [
                {"suit":"CLUBS","value":"K"},
                {"suit":"HEARTS","value":"8"},
                ...
            ]

            
## Levering
* Oppgaven bør leveres i form av en URL til et versjonskontrollert repository, f.eks https://github.com eller https://gitlab.com. Begge tjenester tilbyr gratis repositories.
* Hvis leveringsmåten over ikke fungerer så informere oss gjerne på e-post hvordan du ønsker å levere oppgaven.

## Lykke til :)
