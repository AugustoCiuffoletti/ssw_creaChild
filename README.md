# Creazione di un nuovo componente
Nella app che interroga openweather estraiamo la riga di notifica della temperatura e trasformiamola in un nuovo componente contenuto gerarchicamente nella app-root. Vediamo anche come organizzare la comunicazione dinamica dal padre a figlio.

Articoliamo il procedimento in quattro fasi:

-) Prepariamo l'applicazione creando una classe cityTemp che contiene il contenuto informativo della notifica: nome della città e temperatura. Un nuovo elemento nel template del padre rappresenta il figlio
(branch "creaOggetto")

-) Creiamo il nuovo componente child che chiamiamo "notifica", e trasferiamo codice e template copiandolo dal parent
(branch "creaChild")

-) Creiamo il punto di ingresso della comunicazione da con la direttiva @Input nel controller del figlio ("notifica")
(branch "preparaChild)

-) Creiamo il punto di uscita della comunicazione con un atributo nell'elemento "app-notifica" nel padre (root)
(branch "preparaParent")

Passo successivo sul branch creaOggetto

[Edit on StackBlitz ⚡️](https://stackblitz.com/edit/angular-sswcreachild)