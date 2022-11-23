| Colonna 1 | Colonna 2 |
| --------- | --------- |
| Use case visualizza conto | Visualizzazione del conto  di un tavolo in PDF |
| Goal in Context           | Un supervisore vuole visualizzare il conto di un tavolo, oppure vuole chiudere un conto |
| Preconditions             | Il supervisore ha selezionato dal menù la voce "TAVOLI" |
| Success End Conditions    | La visualizzazione del conto è avvenuta con successo | 
| Failed End Conditions     | E' avvenuto un errore durante la visualizzazione del conto | 
| Primary Actor             | Un supervisore  | 
| Trigger                   | Click sul tavolo di cui si vuole vedere il conto | 

| Description | Step | Supervisore | System |
| ----------- | ---- | ----------- | ------ |
|  | 1 |  | Mostra il menù in formato PDF e l'opzione di chiudere il conto |
|  | 2 | Sceglie di chiudere il conto | |
|  | 3 | | Chiude il conto, e aggiorna il database |

| Extention | Step | User action | System |
| --------- | ---- | ----------- | ------ |
| Il supervisore torna indietro | 1.1 | Il supervisore clicca sul tasto indietro | |
| Errore nella chiusura del conto | 2.1 |  |  | 
