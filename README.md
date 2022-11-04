# Ratatouille23
## Requisiti di sistema 

- Un amministratore può creare per i propri dipendenti (sia addetti alla sala, che addetti alla cucina, che supervisori). Al primo accesso, ogni utente deve re-impostare la password inserita dall'amministratore, scegliendo una password diversa. 


- Un amministratore (o un supervisore) può personalizzare il menù delle attività di ristorazione. Ciascun elemento è caratterizzato da un nome, un costo, una descrizione, e un elenco di allergeni comuni. Inoltre è possibile organizzare gli elementi del menù in categorie personalizzabili (e.g.: primi, dessert, primi di pesce, bibite, etc.), e definire l'ordine con cui gli elementi compaiono nel menù. In fase di inserimento, è richiesto l'autocompletamento di alcuni prodotti (e.g.: bibite o preconfezionati) utilizzando open data come quelli disponibili in https://it.openfoodfacts.org/data.


- Un addetto alla sala può registrare ordinazioni indicando l'identificativo del tavolo e gli elementi del menù desiderati.


- Un supervisore può visualizzare (in formato PDF) il conto di ciascun tavolo in un determinato momento. Inoltre, quando gli avventori seduti ad un certo tavolo vanno via, il supervisore può chiudere il conto e visualizzare la versione finale da sottoporre al cliente.


- Un supervisore o un amministratore può inserire nel sistema degli avvisi, che vengono visualizzati da tutti i dipendenti. Ciascun dipendente può marcare un avviso come "visualizzato" e nasconderlo.


- Un amministratore può visualizzare statistiche sugli introiti dell'attività di ristorazione. In particolare, dato un certo intervallo di tempo personalizzabile, è possibile visualizzare l'incasso medio, il valore medio di ciascun conto, l'incasso complessivo. E' apprezzata la presenza di grafici interattivi.

In particolare, le funzionalità riservate al personale di sala e di cucina saranno fruite su tablet, mentre le funzionalità destinate ad amministratori e supervisori saranno fruite principalmente attraverso notebook o PC. Dal momento che l’hardware (tablet e notebook) non è stato ancora acquistato, si può assumere che su entrambi sia installato un sistema operativo a scelta dei contraenti (e.g.: Linux, Windows, Android, iOS, etc.).
Dato questo insieme di funzionalità, il Committente assegnerà un sottoinsieme non negoziabile di caratteristiche da modellare, implementare e verificare, tenendo in dovuta considerazione il numero di partecipanti al Gruppo di Lavoro contraente.
