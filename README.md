# BalkanAid

**App mobile di supporto per persone in transito sulla rotta balcanica e in Europa.**

BalkanAid offre accesso **offline** a informazioni vitali (assistenza medica, dormitori, supporto legale, emergenze) a migranti e rifugiati che spesso si spostano senza connessione stabile. L'interfaccia è pensata per essere accessibile anche a chi ha poca familiarità con il digitale ed è disponibile in più lingue.

> Questo repository è una vetrina del progetto. Il codice sorgente è privato.

---

## Il problema

Chi attraversa la rotta balcanica ha bisogno di sapere dove trovare cure, un posto per dormire o assistenza legale, ma spesso non ha connessione, non parla la lingua locale e ha poca esperienza con le app. BalkanAid nasce per rendere queste informazioni raggiungibili in modo semplice, affidabile e sicuro.

## Ricerca

La fase di ricerca è stata svolta in collaborazione con una dottoranda in antropologia, attraverso interviste qualitative. I risultati hanno guidato le scelte su contenuti, lingue, semplicità dell'interfaccia e tutela della privacy.

## Funzionalità

- **Mappa offline** basata su OpenStreetMap, consultabile senza connessione
- **Filtri per categoria**: associazioni, ospedali, consolati, polizia, con pin animati e riconoscibili
- **Schede dettagliate** per ogni luogo: orari, contatti, servizi offerti e note importanti
- **Protezione degli indirizzi sensibili**: alcune strutture non mostrano la posizione esatta, per tutelare le persone che le frequentano
- **Multilingua**: inglese e arabo (con supporto alla scrittura da destra a sinistra), farsi in arrivo
- **Dati reali** di organizzazioni attive a Milano (Rete Milano, NAGA)

## Screenshot

<!-- Sostituisci con i tuoi screenshot -->
| Mappa | Filtri | Dettaglio |
|---|---|---|
| ![Mappa](screenshots/mappa.png) | ![Filtri](screenshots/filtri.png) | ![Dettaglio](screenshots/dettaglio.png) |

## Design

Prototipo e interfacce progettati in Figma: [apri il prototipo](INSERISCI-LINK-FIGMA)

Alcune scelte di design hanno una valenza etica diretta: la privacy e la sicurezza degli utenti vengono prima della completezza delle informazioni.

**Palette**

| Ruolo | Colore |
|---|---|
| Primario | `#002455` |
| Secondario | `#6A994E` |
| Accento | `#A7C957` |
| Emergenza | `#BC4749` |

## Tecnologie

- **Flutter** (Android-first)
- **flutter_map** + OpenStreetMap, con cache offline delle mappe
- **Supabase** come backend cloud
- Localizzazione con **flutter_localizations** e file ARB
- **flutter_svg** per icone e pin

## Roadmap

- [ ] Stato aperto/chiuso calcolato dagli orari reali
- [ ] Lingua farsi
- [ ] Sezione luoghi salvati
- [ ] App separata per i volontari, con accesso solo su invito
- [ ] Mappa offline dell'intera rotta balcanica

## Ruolo

Progetto personale. Ho curato UX/UI, prototipazione in Figma e sviluppo, e ho condotto la ricerca con interviste insieme a una dottoranda in antropologia. Tutte le decisioni su priorità, esperienza utente e dati sono mie.

---

Margherita · [contatti](INSERISCI-LINK-O-EMAIL)
