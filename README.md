# Ratatouille23
| Giorno | Aggiornamento |
| ------ | ------------- |
|  09/11/22 | Use case diagrams |
| 10/11/22 | Boh |
| 12/11/22 | Individuazione del target degli utenti |

## Cose da fare:
1. Vedere ListView ruolo in class creaUtente
2. Cambiare nome nel button invece di login in creaUtente
3. Aggiungere button torna indietro

## Output
Per le attività sopracitate, il Committente richiede i seguenti output:
1. Documento dei Requisiti Software
  - a Analisi dei Requisiti
    - -[x] i Modellazione di tutti i casi d’uso richiesti.
    - -[x] ii Individuazione del target degli utenti. (solo gruppi “Nuovo Ordinamento”)
    - -[x] iii Descrizioni Testuali Strutturate per almeno quattro (due, se si consegna prima del
      31/03/2023) casi d’uso significativi (autenticazione esclusa) a scelta dei contraenti
      tra quelli richiesti.
    - -[x] iv Prototipazione visuale via Mock-up dell’interfaccia utente per tutti i casi d’uso
      assegnati. Si raccomanda caldamente l’uso del tool “Figma”.
    - -[ ] v Valutazione dell’usabilità a priori. (solo gruppi “Nuovo Ordinamento”)
    - -[ ] vi Glossario.
  - b Specifica dei Requisiti.
    - -[ ] i Classi, oggetti e relazioni di analisi.
    - -[ ] ii Diagrammi di sequenza di analisi per due casi d’uso significativi a scelta dei
      contraenti tra quelli assegnati.
    - -[ ] iii Prototipazione funzionale via statechart dell’interfaccia grafica, relativamente ai casi
      d’uso individuati al punto 1.a.iii; (solo gruppi “Nuovo Ordinamento”)

2. Documento di Design del sistema.
  - -[ ] a Analisi dell’architettura con esplicita definizione dei criteri di design.
  - -[ ] b Descrizione/motivazione delle scelte tecnologiche adottate.
  - -[ ] c Diagramma delle classi di design.
  - -[ ] d Diagrammi di stato di design, ove non banali (solo gruppi “Vecchio Ordinamento”).
  - -[ ] e Diagrammi di sequenza di design per i casi d’uso identificati al punto 1.a.iii.

3. Codice Sorgente sviluppato, comprensivo di eventuale Dockerfile.

4. Testing e valutazione sul campo dell’usabilità.
  - -[ ] a Codice xUnit per unit testing di quattro (due, se si consegna prima del 31/03/2023) metodi
    non banali, che abbiano almeno due parametri. In aggiunta al codice, una apposita sezione
    della documentazione deve descrivere le strategie adottate per la progettazione dei test dei
    due metodi (e.g.: classi di equivalenza individuate e coperte, criteri di copertura strutturale,
    etc.).
  - -[ ] b Valutazione dell’usabilità sul campo, realizzata sul prodotto finito sia con tecniche simili a
    quelle messe in atto al punto 1.a.v, sia mediante analisi di file di log. È necessario allegare
    anche i file di log utilizzati nell’analisi. (solo gruppi “Nuovo Ordinamento”)
    Si noti che i Punti 1, 2 e 4 vanno realizzati come un unico documento, di seguito indicato come
    “documentazione”.

## Requisiti di sistema 

- Un amministratore può creare per i propri dipendenti (sia addetti alla sala, che addetti alla cucina, che supervisori). Al primo accesso, ogni utente deve re-impostare la password inserita dall'amministratore, scegliendo una password diversa. 


- Un amministratore (o un supervisore) può personalizzare il menù delle attività di ristorazione. Ciascun elemento è caratterizzato da un nome, un costo, una descrizione, e un elenco di allergeni comuni. Inoltre è possibile organizzare gli elementi del menù in categorie personalizzabili (e.g.: primi, dessert, primi di pesce, bibite, etc.), e definire l'ordine con cui gli elementi compaiono nel menù. In fase di inserimento, è richiesto l'autocompletamento di alcuni prodotti (e.g.: bibite o preconfezionati) utilizzando open data come quelli disponibili in https://it.openfoodfacts.org/data.


- Un addetto alla sala può registrare ordinazioni indicando l'identificativo del tavolo e gli elementi del menù desiderati.


- Un supervisore può visualizzare (in formato PDF) il conto di ciascun tavolo in un determinato momento. Inoltre, quando gli avventori seduti ad un certo tavolo vanno via, il supervisore può chiudere il conto e visualizzare la versione finale da sottoporre al cliente.


- Un supervisore o un amministratore può inserire nel sistema degli avvisi, che vengono visualizzati da tutti i dipendenti. Ciascun dipendente può marcare un avviso come "visualizzato" e nasconderlo.


- Un amministratore può visualizzare statistiche sugli introiti dell'attività di ristorazione. In particolare, dato un certo intervallo di tempo personalizzabile, è possibile visualizzare l'incasso medio, il valore medio di ciascun conto, l'incasso complessivo. E' apprezzata la presenza di grafici interattivi.

In particolare, le funzionalità riservate al personale di sala e di cucina saranno fruite su tablet, mentre le funzionalità destinate ad amministratori e supervisori saranno fruite principalmente attraverso notebook o PC. Dal momento che l’hardware (tablet e notebook) non è stato ancora acquistato, si può assumere che su entrambi sia installato un sistema operativo a scelta dei contraenti (e.g.: Linux, Windows, Android, iOS, etc.).
Dato questo insieme di funzionalità, il Committente assegnerà un sottoinsieme non negoziabile di caratteristiche da modellare, implementare e verificare, tenendo in dovuta considerazione il numero di partecipanti al Gruppo di Lavoro contraente.

## Requisiti di dominio
Tutte le funzionalità assegnate devono essere realizzate implementando un sistema distribuito in cui è possibile individuare due macro-componenti:
- una parte front-end, comprensiva delle interfacce utente;
- una parte back-end, che espone delle API REST che vengono utilizzate dal front-end.

È altresì auspicabile che il back-end sia distribuito come container Docker e che, al momento della discussione del progetto con demo del prodotto, sia messo in opera (utilizzando tecnologie allo stato dell’arte quali ad esempio servizi di public Cloud Computing come Azure o AWS), e sia quindi accessibile attraverso la rete Internet.
Per lo svolgimento delle attività di progettazione, è obbligatorio l’utilizzo di tool di CASE. Inoltre, si richiede tassativamente di astrarre il design per favorire il riutilizzo del codice e la futura implementazione di altre funzionalità, esplicitando nella documentazione (si veda Sezione 5) le scelte intraprese per favorire tale astrazione.
Per quanto riguarda le tecnologie da utilizzare, è data piena libertà di scelta al Gruppo di Lavoro contraente, con l’unico vincolo dell’utilizzo obbligatorio di linguaggi di programmazione Object- Oriented. Per esempio, la parte front-end può essere realizzata come applicazione desktop (e.g.: con

## Altro

| ID | Requisito |
| -- | --------- |
| crea utenza | Un amministratore può creare utenza per i propri dipendenti(sia addetti alla sala, che addetti alla cucina, che supervisori). Al primo accesso, ogni utente deve re-impostare la password inserita dall'amministratore, scegliendo una password diversa. |
| personalizza menu |  Un amministratore (o un supervisore) può personalizzare il menù delle attività di ristorazione. Ciascun elemento è caratterizzato da un nome, un costo, una descrizione, e un elenco di allergeni comuni. Inoltre è possibile organizzare gli elementi del menù in categorie personalizzabili (e.g.: primi, dessert, primi di pesce, bibite, etc.), e definire l'ordine con cui gli elementi compaiono nel menù. In fase di inserimento, è richiesto l'autocompletamento di alcuni prodotti (e.g.: bibite o preconfezionati) utilizzando open data come quelli disponibili in https://it.openfoodfacts.org/data |
| registra ordinazione | Un addetto alla sala può registrare ordinazioni indicando l'identificativo del tavolo e gli elementi del menù desiderati | 
| visualizza conto | Un supervisore può visualizzare (in formato PDF) il conto di ciascun tavolo in un determinato momento. Inoltre, quando gli avventori seduti ad un certo tavolo vanno via, il supervisore può chiudere il conto e visualizzare la versione finale da sottoporre al cliente |
| invia notifica | Un supervisore o un amministratore può inserire nel sistema degli avvisi, che vengono visualizzati da tutti i dipendenti. Ciascun dipendente può marcare un avviso come "visualizzato" e nasconderlo | 
| visualizza statistiche | Un amministratore può visualizzare statistiche sugli introiti dell'attività di ristorazione. In particolare, dato un certo intervallo di tempo personalizzabile, è possibile visualizzare l'incasso medio, il valore medio di ciascun conto, l'incasso complessivo. E' apprezzata la presenza di grafici interattivi |

## Link utili
https://fireship.io
https://www.youtube.com/watch?v=Sh6lK57Cuk4&list=PL0vfts4VzfNixzfaQWwDUg3W5TRbE7CyI
https://code.visualstudio.com/docs/nodejs/working-with-javascript

https://www.overleaf.com/5541297171dhdhtvymwxbc
https://www.figma.com/team_invite/redeem/A4K8LucOmHwZczIw8DMXGf
https://iconduck.com/icons/113753/pound-coin
