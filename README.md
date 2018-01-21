# Oving4
Øving 4 - Databaser og systemutvikling


Øving 4TDAT1005 Databaser med videregående programmeringInstitutt for datateknologi og informatikk (IDI), NTNU
Mer om programmering av aggregeringer


Du skal jobbe med et system for reservering av rom i et konferansesenter.
Konferansesenteret har mange møterom, og hvert rom har et nummer (heltall) og en størrelse. Størrelsen er angitt i antall personer det er plass til i rommet. En reservasjon består av to tidspunkter (fra og til), samt navn og telefonnr til kunden.


Klassen Reservasjon er gitt. En reservasjon består av et tidsintervall gitt ved to tidspunkt (fra - til). Klassen tilbyr blant annet en metode som sjekker om et annet tidsintervall overlapper med dette. Den metoden trenger du når du skal finne om et rom er ledig på et bestemt tidspunkt.

Reservasjon bruker klassene Kunde og Tidspunkt.
Vi lagrer et tidspunkt som et heltall (datatypen long), eksempel 200301201230L, betyr 20. januar 2003, kl 12:30. Ved å lagre tidspunkt på denne måten kan du finne ut om et tidspunkt er før eller etter et annet ved enkel sammenligning. Klassen Tidspunkt har en toString()-metode som kan brukes til å få skrevet ut tidspunktet på en lettere lesbar form.


En klient vil i hovedsak forholde seg til et Konferansesenter-objekt. Et slikt objekt skal tilby følgende tjenester

Reserver rom, gitt tidspunkt fra og til, antall personer samt navn og telefonnummer til kunden. (Her skal romnummer ikke være parameter, metoden skal selv finne et rom som er ledig og med plass til det oppgitte antallet personer.)

Registrer et nytt rom med romnummer og størrelse (ikke tillatt dersom rom med dette nummer fins fra før)
Finn antall rom
Finn et bestemt rom, gitt indeks
Finn et bestemt rom, gitt romnr

Du kan gjerne la klassene tilby flere metoder enn angitt over.

Du må selv finne ut hvilke tjenester klassen Rom skal tilby.


Forslag til angrepsmåte:
Gjør deg kjent med de tre klassene som er gitt. Legg merke til at det følger med testprogram ved at main() er lagt inne i klassene. Du trenger ikke ta bort dette for å bruke klassene.

Inne i klassen Konferansesenter skal du ha en ArrayList av romobjekter. Skisser metodene i klassen Konferansesenter. Det bør gi ideer til hvilke metoder du trenger i klassen Rom.

Inne i klassen Rom skal du ha en ArrayList av reservasjonsobjekter. Programmer metodene i klassen Rom. Lag et testprogram for denne klassen på tilsvarende måte som det er gjort for de klassene som er gitt. Prøv ut at metodene virker, f.eks. om de håndterer overlapp i tid ved reservasjon av rommet.

Programmer metodene i klassen Konferansesenter.
Lag et klientprogram der brukeren kan legge inn data. Sørg for at alle metodene i klassen Konferansesenter blir prøvd ut.
Begynn med å registrere alle rommene.
Les inn noen reservasjoner.
Skriv ut all registrert informasjon. Bruk metodene som finner antall rom og rom gitt indeks.
Prøv ut metoden som finnet er rom, gitt romnummer. La brukeren skrive inn romnummeret. All info om rommet, inkludert reservasjonene skal skrives ut.

Du skal levere:
klassen Rom med eget testprogram, se pkt. 3 foran
klassen Konferansesenter
klientprogrammet etter malen gitt under pkt. 5 foran (eller mer avansert)
Lykke til!
