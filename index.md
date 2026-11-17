# Privacy Policy — Hangar Pro

_Ultimo aggiornamento: 17 novembre 2026_ · [English below](#english)

**Hangar Pro** è un'app per seguire e guidare dal telefono le sessioni di Claude Code che girano sui
propri computer. Su ogni computer gira un programma, il Node di Hangar Pro, che tiene le sessioni.
L'app parla solo con i Node che l'utente associa: il titolare non ha server, non ha account utente e
non riceve nessun dato dall'app.

## Dati trattati

- **Contenuto delle sessioni:** conversazioni, terminale, nomi e cartelle delle sessioni, foto e file
  allegati, testo dettato. Vanno solo al Node dei computer dell'utente, agli indirizzi che inserisce lui
  (in rete locale o attraverso una sua VPN). Il collegamento è **cifrato (TLS)** e l'app accetta solo il
  certificato del Node associato, verificato con la sua impronta.
- **Elenco dei computer associati e chiavi per collegarsi:** restano sul telefono, fuori dal backup di
  Android e dal trasferimento a un altro telefono.
- **Token di notifica (Firebase Cloud Messaging):** un identificativo tecnico del dispositivo, ottenuto da
  Google e consegnato ai Node dell'utente, usato **esclusivamente** per recapitare gli avvisi all'app.

## Cosa passa da Google

- **Notifiche (Firebase Cloud Messaging).** Quando una sessione aspetta l'utente, il Node manda a Google,
  perché lo recapiti al telefono, solo il nome della sessione, il nome del computer, un identificativo
  della sessione, il tipo di avviso e un testo fisso (per esempio "Ti aspetta"). **Mai** il testo della
  conversazione o del terminale. Il messaggio dura al più un'ora.
- **Lettura del QR (ML Kit).** Il QR per associare un computer si legge sul telefono. La libreria ML Kit di
  Google manda a Google dati di diagnostica e di uso (modello e versione del sistema del telefono, nome e
  versione dell'app, un identificativo dell'installazione, tempi di risposta, formato e dimensione delle
  immagini analizzate, codici d'errore); secondo la documentazione di Google non manda le immagini né il
  contenuto del QR. Il QR si può evitare inserendo a mano indirizzo e codice.

Google tratta questi dati secondo le proprie norme: <https://policies.google.com/privacy>.

## Permessi

- **Fotocamera:** per inquadrare il QR di associazione e per scattare una foto da allegare, solo quando lo
  chiede l'utente. Le foto sono ridotte e private dei dati EXIF e della posizione prima di partire verso il Node.
- **Microfono:** solo per la dettatura, con il riconoscitore vocale sul dispositivo. L'audio non esce dal
  telefono.
- **Notifiche:** per gli avvisi delle sessioni. **Rete:** per collegarsi ai Node dell'utente.
- Foto e file da allegare si scelgono con il selettore di Android: l'app vede solo quelli scelti.

## Dati NON raccolti

L'app **non** raccoglie posizione, contatti, dati biometrici, dati finanziari o dati relativi alla salute,
e **non** integra servizi propri di analisi o pubblicità.

## Condivisione e finalità

I dati **non** vengono venduti né ceduti e **non** sono usati per pubblicità o profilazione. Sono trattati
al solo scopo di far funzionare l'app. L'app non è rivolta ai minori.

## Conservazione e cancellazione

Il contenuto delle sessioni resta sui computer dell'utente. Disinstallando l'app si cancellano dal telefono
l'elenco dei computer, le chiavi e il token di notifica; da ogni Node si può revocare in qualsiasi momento un
dispositivo associato. Il titolare non conserva dati da cancellare.

## Titolare e contatto

Emanuele Perini — perini@vision-e.it

---

## English

_Last updated: 17 November 2026_

**Hangar Pro** lets you follow and drive, from your phone, the Claude Code sessions running on your own
computers. Each computer runs the Hangar Pro Node, which holds the sessions. The app talks only to the Nodes
you pair: the developer has no server, no user accounts and receives no data from the app.

- **Session content** (conversations, terminal, session names and folders, attached photos and files,
  dictated text) goes only to your own Nodes, at the addresses you enter, over **TLS** pinned to the paired
  Node's certificate. The list of paired computers and the connection keys stay on the phone, excluded from
  Android backup and device transfer.
- **Notifications (Firebase Cloud Messaging):** the app gets a push token from Google and hands it to your
  Nodes. A notification carries only the session name, the computer name, a session id, the alert type and a
  fixed text — never conversation or terminal text — and expires within one hour.
- **QR scanning (ML Kit):** Google's ML Kit sends Google diagnostic and usage data (device model and OS
  version, app name and version, an installation id, latency, image format and size, error codes); per
  Google's documentation, not the images or the QR content. You can avoid it by entering address and code by
  hand. Google's policy: <https://policies.google.com/privacy>.
- **Permissions:** camera (QR and photos you take, stripped of EXIF and location), microphone (on-device
  dictation only; audio never leaves the phone), notifications, network.
- No location, contacts, biometric, financial or health data; no own analytics or ads; no sale or transfer of
  data; not directed at children.
- Uninstalling the app removes paired computers, keys and the push token from the phone; any Node can revoke a
  paired device at any time. The developer holds no data to delete.

**Controller and contact:** Emanuele Perini — perini@vision-e.it
