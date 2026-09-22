# Referto Pallanuoto — installazione su iPhone, iPad e Mac

Questa versione è una **PWA**: non deve essere pubblicata sull'App Store.

## 1. Pubblicare la cartella online

La cartella `pwa19` deve essere pubblicata su un indirizzo **HTTPS**. Per esempio puoi usare GitHub Pages.

### GitHub Pages
1. Crea un account GitHub, se non ne hai già uno.
2. Crea un nuovo repository, ad esempio `referto-pallanuoto`.
3. Carica **il contenuto della cartella `pwa19`** nel repository, quindi `index.html`, `app.js`, `styles.css`, `manifest.webmanifest`, `sw.js` e le icone devono trovarsi nella cartella principale pubblicata.
4. In **Settings → Pages**, abilita la pubblicazione da branch `main` e cartella `/root`.
5. Attendi la pubblicazione e apri l'indirizzo HTTPS generato.

> Importante: il servizio deve usare HTTPS. Il service worker e l'installazione PWA non funzionano correttamente da un normale file `file://`.

## 2. Installazione su iPhone

1. Apri l'indirizzo della PWA in **Safari**.
2. Tocca **Condividi**.
3. Scegli **Aggiungi alla schermata Home**.
4. Lascia il nome `Referto Pallanuoto`.
5. Tocca **Aggiungi**.
6. Apri l'icona dalla Home.

## 3. Installazione su iPad

1. Apri la PWA in **Safari**.
2. Tocca **Condividi**.
3. Scegli **Aggiungi alla schermata Home**.
4. Tocca **Aggiungi**.

L'app si aprirà in modalità standalone, senza la normale barra degli indirizzi del browser.

## 4. Installazione su Mac

Con una versione recente di macOS/Safari:

1. Apri la PWA in Safari.
2. Usa il menu **File** oppure **Condividi**.
3. Scegli l'opzione per **Aggiungere al Dock** / aggiungere il sito come app, quando disponibile.
4. Conferma il nome `Referto Pallanuoto`.

In alternativa puoi continuare a usare la PWA direttamente da Safari.

## 5. Funzionamento offline

Dopo la prima apertura online, la PWA memorizza i file principali tramite il service worker. Le partite e le impostazioni già salvate nell'app restano nei dati locali del dispositivo.

Per sicurezza usa periodicamente il pulsante **Esporta backup** presente nell'app e conserva il file JSON.

## 6. Aggiornamenti

Quando viene pubblicata una nuova versione del progetto, il service worker utilizza una nuova cache. Chi ha già installato la PWA può doverla aprire con connessione internet almeno una volta per ricevere l'aggiornamento.
