# Kjøleskapsapp

Dette prosjektet er en desktopapplikasjon utviklet i Java med JavaFX, som gir brukeren oversikt over matvarene i kjøleskapet. Appen lar brukeren legge til, fjerne og administrere matvarer, samt lagre og laste inn kjøleskapets innhold.

Prosjektet ble utviklet som en del av emnet TDT4100 – Objektorientert programmering ved NTNU våren 2024.

## Funksjonalitet

- **Legge til matvarer:** Registrer matvarer med navn, kategori og antall.
- **Fjerne matvarer:** Reduser antallet eller fjern en matvare helt fra kjøleskapet.
- **Kategorisering:** Organiser matvarer i kategoriene Pålegg, Drikke, Grønnsaker, Saus og Annet.
- **Automatisk oppdatering:** Hvis en matvare legges til på nytt i samme kategori, økes antallet på den eksisterende matvaren.
- **Lagring og innlasting:** Lagre kjøleskapets innhold til en CSV-fil og last inn tidligere lagrede matvarer.
- **Oversikt:** Se totalt antall matvarer og antall matvarer i hver kategori.
- **Feilhåndtering:** Få tilbakemeldinger ved ugyldige handlinger, for eksempel manglende kategori, forsøk på å laste inn et tomt kjøleskap eller forsøk på å fjerne flere varer enn det som finnes.

## Teknologier

- Java
- JavaFX
- FXML
- CSV-filbehandling
- JUnit for enhetstesting

## Struktur og design

Prosjektet benytter objektorienterte prinsipper for å organisere kode og funksjonalitet.

- **Model:** `Matvare` representerer en matvare, mens `KjoeleskapBehandler` håndterer logikken for å administrere matvarene.
- **View:** `App.fxml` definerer brukergrensesnittet.
- **Controller:** `KjoeleskapController` håndterer brukerinteraksjoner og kobler sammen brukergrensesnittet og applikasjonslogikken.
- **Interface:** `Kjoeleskap` definerer funksjonalitet for lagring og innlasting, som implementeres av `CSVKjoeleskap`.
- **Filhåndtering:** Matvarene lagres og leses fra en CSV-fil.
- **Testing:** Enhetstester brukes til å kontrollere sentral funksjonalitet og håndtere ugyldige verdier.

## Hva jeg lærte

Gjennom prosjektet fikk jeg praktisk erfaring med objektorientert programmering og utvikling av grafiske applikasjoner i Java. Jeg jobbet blant annet med klasser og objekter, interfaces, unntakshåndtering, lambda-uttrykk, filhåndtering og enhetstesting.

Prosjektet ga meg også erfaring med Model-View-Controller-prinsippet (MVC). 

## Mulige videreutviklinger

- Sortering av matvarer etter navn, kategori eller antall.
- Registrering av utløpsdatoer for å bidra til mindre matsvinn.
- Videre forbedring av MVC-strukturen.
- Utvidet testdekning for controller og brukergrensesnitt.

