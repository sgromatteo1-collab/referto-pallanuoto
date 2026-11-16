# Match – aggiornamento statistiche e mappa porta (16 novembre 2026)

## Novità
- Riepilogo squadra ricalcolato da tutti gli eventi: goal, tiri, tiri sbagliati, fuori, parate, gol subiti, assist, efficacia.
- Goal subiti dei portieri attribuiti solo a eventi registrati sulla calotta del portiere interessato. Se un evento è assegnato per errore a una non-portiera, appare un avviso di riconciliazione.
- Eliminazione sicura: apri un evento dall'elenco, seleziona Elimina, conferma; il pulsante **Annulla eliminazione** ripristina l'ultimo evento rimosso.
- Localizzazione: nell'evento Tiro / Goal scegli **Apri porta**, tocca un punto sulla porta o fuori dai pali e conferma. Si registrano percentuali X/Y e zona (sei zone interne o fuori).
- Le statistiche squadra e individuali comprendono tiri sbagliati, tiri fuori, tiri ricevuti e parate. Il riepilogo zone include i vecchi tiri privi di posizione sotto **Non localizzato**.
- Cronologia PDF ed Excel riportano la zona di tiro (Excel comprende coordinate).

## Uso e compatibilità
Usa la stessa origine/indirizzo dell'installazione precedente: i dati rimangono nella chiave localStorage `referto-pallanuoto-v12`. Per sicurezza esporta prima un backup JSON dalla versione precedente. Le partite archiviate conservano il loro snapshot e non vengono modificate finché non vengono aperte e salvate nuovamente.

La posizione dei tiri storici non è ricostruibile automaticamente. La porta rappresenta una vista schematica frontale, non una misurazione sportiva omologata. Verifica su dispositivo reale l'installazione PWA, l'archiviazione locale e l'esportazione.

## Calotta marcatrice avversaria
Quando registri **Goal subito** su un portiere puoi indicare la calotta (1–99) della marcatrice avversaria. Il valore è modificabile riaprendo l’evento e viene salvato insieme al gol, riportato nella cronologia e nelle esportazioni PDF/Excel. È opzionale per i dati storici e non crea un secondo evento: punteggio e gol subiti vengono conteggiati una sola volta.
