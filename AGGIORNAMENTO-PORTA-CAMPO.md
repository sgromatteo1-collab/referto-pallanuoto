# Match – aggiornamento porta e mappa controfalli (16 novembre 2026)

- Porta graficamente rinnovata: pali bianchi e rossi, rete tridimensionale, acqua, sei zone e area esterna per i tiri fuori.
- Coordinate precedenti mantenute (stessa scala 0–100 e stessi limiti zona).
- Mappa top-down del campo: tocca il punto per controfalli guadagnati o subiti, con suddivisione in attacco, centrocampo, difesa e lato sinistro/centrale/destro.
- La posizione viene memorizzata dentro l’evento (fieldPosition), mostrata nell’elenco eventi e nel riepilogo statistico di squadra. Gli stessi eventi alimentano le statistiche individuali.
- In modifica evento la posizione già registrata viene ripristinata; eliminando l’evento si ricalcolano anche i dati per zona.
- La mappa usa la convenzione visiva porta avversaria in alto / porta nostra in basso.
- Aggiornata cache PWA per evitare stili/script vecchi.

## Revisione grafica sulla base del riferimento fornito
- Campo riprogettato in vista dall’alto con delimitazioni, due porte con rete, metà campo, cerchio centrale e bande colorate laterali.
- Invariati area cliccabile, scala delle coordinate e calcolo delle statistiche; nessuna conversione dell’archivio necessaria.

## Rifinitura porta v4
- Etichetta superiore cambiata in FUORI.
- Rimossa ogni scritta nell’acqua sotto la porta e migliorata la grafica delle onde.
- Conservate coordinate, zone e comportamento dei tiri fuori.
