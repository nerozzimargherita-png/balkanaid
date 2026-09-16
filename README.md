# BalkanAid

App Android per chi è in transito sulla rotta balcanica: dove trovare un medico, un posto per dormire, un'associazione o un aiuto legale, anche senza connessione.
Il codice è in un repository privato. Qui trovi una panoramica del progetto e il link al prototipo.

### Perché

Chi attraversa i Balcani spesso non ha internet, non parla la lingua del posto e usa poco le app. Le informazioni utili esistono, ma sono sparse e difficili da trovare. BalkanAid prova a metterle in un unico posto, consultabile offline e in inglese, arabo e (a breve) farsi.


### Ricerca

Prima di progettare ho svolto una ricerca in due parti, in collaborazione con una dottoranda in antropologia.
La parte qualitativa è composta da interviste approfondite, di almeno un'ora ciascuna, a presidenti di associazioni umanitarie attive sulla rotta balcanica e a migranti. La parte quantitativa è un questionario online, diffuso tra persone che avevano già percorso la rotta.
Da questo lavoro sono derivate molte scelte del progetto: i contenuti, le lingue, un'interfaccia essenziale con icone al posto del testo dove possibile, e l'attenzione alla privacy.

### Funzionalità

- Mappa basata su OpenStreetMap, consultabile senza connessione
- Filtri per categoria (associazioni, ospedali, consolati, polizia) con pin riconoscibili
- Schede per ogni luogo con orari, contatti, servizi e note importanti
- Indirizzi sensibili nascosti, per tutelare le persone che frequentano alcune strutture
- Inglese e arabo, con supporto alla scrittura da destra a sinistra; farsi in arrivo
- Dati reali di realtà attive a Milano, come Rete Milano e NAGA

### Design

Wireframe e prototipo su [Figma](https://www.figma.com/design/irABRiS6epvZDJeTblttPh/BalkanAid---Wireframe-v1?node-id=0-1).

### Tecnologie

Flutter (Android-first), flutter_map con OpenStreetMap e cache offline, Supabase come backend, Hive per i dati offline, geolocalizzazione GPS, flutter_localizations con file ARB, flutter_svg per icone e pin.

### Struttura del codice

    lib/
    ├── l10n/        traduzioni (file ARB)
    ├── models/      modelli dati: luoghi, organizzazioni, categorie
    ├── screens/     schermate dell'app
    ├── services/    connessione a Supabase e gestione della cache offline
    ├── theme/       colori, tipografia e stili
    ├── widgets/     componenti riutilizzabili (pin, filtri, schede)
    └── main.dart    punto di ingresso dell'app

### Ruolo

Progetto personale. Ho curato ricerca, UX/UI, prototipazione in Figma e sviluppo. Tutte le decisioni su priorità, esperienza utente e dati sono mie.
