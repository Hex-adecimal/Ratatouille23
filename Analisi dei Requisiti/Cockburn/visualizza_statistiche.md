| Colonna 1 | Colonna 2 |
| --------- | --------- |
| Use case visualizza statistiche | Visualizzazione delle statistiche di vendita |
| Goal in Context | L'amministratore vuole visualizzare le statistiche di vendità del ristorante |
| Preconditions   | L'amministratore si trova nell'interfaccia di visualizzazione statistiche |
| Success End Conditions | Le statistiche vengono visualizzate con successo | 
| Failed End Conditions | Non è stato possibile visualizzare le statistiche | 
| Primary Actor | L'amministratore  | 
| Trigger | Clicca sulla scritta "HOME" | 

| Description | Step | Amministratore | System |
| ----------- | ---- | -------------- | ------ |
|  | 1 | Click sulla scritta "HOME" |  |
|  | 2 |  | Restituisce le statistiche comprese nell'intervallo di tempo \[t0,ADESSO\] |

| Extention | Step | User action | System |
| --------- | ---- | ----------- | ------ |
|  | 2.1 | Seleziona un diverso intervallo di tempo | |
|  | 2.2 | | Restituisce le statistiche comprese nell'intervallo di tempo inserito |
