Termine: requests (Libreria [[Python]])

Descrizione:
requests è una libreria di terze parti per [[Python]] estremamente popolare, progettata per effettuare richieste HTTP in modo semplice e leggibile. Permette a un programma di comunicare con siti web e [[API]] (ad esempio per scaricare dati, leggere pagine web o inviare moduli) senza doversi preoccupare della complessa gestione a basso livello delle connessioni di rete, semplificando enormemente l'interazione con il web.

Contesto:
Sviluppo web, web scraping, automazione di rete e integrazione con [[API]] RESTful.

Esempio:
Scrivendo risposta = requests.get("https://[[api]].meteo.it/roma"), il tuo script si collega istantaneamente al server per scaricare i dati meteorologici correnti, permettendoti di estrarli subito in un formato comodo usando il comando risposta.[[json]]().