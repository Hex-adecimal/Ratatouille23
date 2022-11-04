# Ratatouille23
## Obiettivi
Per la realizzazione del suddetto obiettivo, SoftEngUniNA richiede la progettazione, implementazione e parziale verifica dei moduli software necessari al corretto funzionamento dei sistemi informatici.
### Analisi e specifica dei requisiti

### Definizione dell’architettura e progettazione del sistema

### Implementazione del sistema

### Testing e valutazione sul campo dell’usabilità

## Requisiti

### Requisiti di sistema 

- Un amministratore può creare per i propri dipendenti (sia addetti alla sala, che addetti alla cucina, che supervisori). Al primo accesso, ogni utente deve re-impostare la password inserita dall'amministratore, scegliendo una password diversa. 


- Un amministratore (o un supervisore) può personalizzare il menù delle attività di ristorazione. Ciascun elemento è caratterizzato da un nome, un costo, una descrizione, e un elenco di allergeni comuni. Inoltre è possibile organizzare gli elementi del menù in categorie personalizzabili (e.g.: primi, dessert, primi di pesce, bibite, etc.), e definire l'ordine con cui gli elementi compaiono nel menù. In fase di inserimento, è richiesto l'autocompletamento di alcuni prodotti (e.g.: bibite o preconfezionati) utilizzando open data come quelli disponibili in https://it.openfoodfacts.org/data.


- Un addetto alla sala può registrare ordinazioni indicando l'identificativo del tavolo e gli elementi del menù desiderati.


- Un supervisore può visualizzare (in formato PDF) il conto di ciascun tavolo in un determinato momento. Inoltre, quando gli avventori seduti ad un certo tavolo vanno via, il supervisore può chiudere il conto e visualizzare la versione finale da sottoporre al cliente.


- Un supervisore o un amministratore può inserire nel sistema degli avvisi, che vengono visualizzati da tutti i dipendenti. Ciascun dipendente può marcare un avviso come "visualizzato" e nasconderlo.


- Un amministratore può visualizzare statistiche sugli introiti dell'attività di ristorazione. In particolare, dato un certo intervallo di tempo personalizzabile, è possibile visualizzare l'incasso medio, il valore medio di ciascun conto, l'incasso complessivo. E' apprezzata la presenza di grafici interattivi.

In particolare, le funzionalità riservate al personale di sala e di cucina saranno fruite su tablet, mentre le funzionalità destinate ad amministratori e supervisori saranno fruite principalmente attraverso notebook o PC. Dal momento che l’hardware (tablet e notebook) non è stato ancora acquistato, si può assumere che su entrambi sia installato un sistema operativo a scelta dei contraenti (e.g.: Linux, Windows, Android, iOS, etc.).
Dato questo insieme di funzionalità, il Committente assegnerà un sottoinsieme non negoziabile di caratteristiche da modellare, implementare e verificare, tenendo in dovuta considerazione il numero di partecipanti al Gruppo di Lavoro contraente.

### Requisiti di dominio
Tutte le funzionalità assegnate devono essere realizzate implementando un sistema distribuito in cui è possibile individuare due macro-componenti:
• una parte front-end, comprensiva delle interfacce utente;
• una parte back-end, che espone delle API REST che vengono utilizzate dal front-end.
È altresì auspicabile che il back-end sia distribuito come container Docker e che, al momento della discussione del progetto con demo del prodotto, sia messo in opera (utilizzando tecnologie allo stato dell’arte quali ad esempio servizi di public Cloud Computing come Azure o AWS), e sia quindi accessibile attraverso la rete Internet.
Per lo svolgimento delle attività di progettazione, è obbligatorio l’utilizzo di tool di CASE. Inoltre, si richiede tassativamente di astrarre il design per favorire il riutilizzo del codice e la futura implementazione di altre funzionalità, esplicitando nella documentazione (si veda Sezione 5) le scelte intraprese per favorire tale astrazione.
Per quanto riguarda le tecnologie da utilizzare, è data piena libertà di scelta al Gruppo di Lavoro contraente, con l’unico vincolo dell’utilizzo obbligatorio di linguaggi di programmazione Object- Oriented. Per esempio, la parte front-end può essere realizzata come applicazione desktop (e.g.: con

## Link utili
https://fireship.io
https://www.youtube.com/watch?v=Sh6lK57Cuk4&list=PL0vfts4VzfNixzfaQWwDUg3W5TRbE7CyI
https://code.visualstudio.com/docs/nodejs/working-with-javascript

