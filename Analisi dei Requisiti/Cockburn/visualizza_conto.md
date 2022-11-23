| Colonna 1 | Colonna 2 |
| --------- | --------- |
| Use case crea utenza | Registrazione utenza |
| Goal in Context | L'amministratore vuole registrare un nuovo dipendente |
| Preconditions   | Il dipendente non è stato registrato e l'amministratore si trova nella schermata di registrazione dell'utente  |
| Success End Conditions | La registrazione è avvenuta con successo| 
| Failed End Conditions | Non è stato possibile effettuare la registrazione | 
| Primary Actor | L'amministratore  | 
| Trigger | Clicca sulla scritta "CREA UTENTE" | 

| Description | Step | Amministratore | System |
| ----------- | ---- | -------------- | ------ |
|  | 1 | Click sulla scritta "CREA UTENTE" dalla schermata home |  |
|  | 2 | | Mostra la schermata di creazione di un dipendente |
|  | 3 | Inserisce le informazioni nei campi |  |
|  | 4 | Click sul bottone "CREA UTENTE" | |
|  | 5 | | Controlla se l'username non esiste già nel database |
|  | 6 | | Controlla se la password abbia almeno 8 caratteri |
|  | 7 | | Registra l'utente |

| Extention | Step | User action | System |
| --------- | ---- | ----------- | ------ |
| L'username è già usato | 5.1 | | Mostra errore ”USERNAME NON DISPONIBILE” all’interno della schermata "CREAZIONE DEL DIPENDENTE" |
| La password ha meno di 8 caratteri | 6.1 | | Mostra errore ”PASSWORD NON VALIDA” all’interno della schermata "CREAZIONE DEL DIPENDENTE" |
