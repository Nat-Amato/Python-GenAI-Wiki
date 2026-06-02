Termine: REST [[API]] - Metodi (GET, POST, PUT, DELETE)

Descrizione:
Le REST [[API]] utilizzano i metodi standard del protocollo HTTP per compiere le quattro operazioni fondamentali sui dati (spesso chiamate CRUD: Create, Read, Update, Delete). GET serve esclusivamente per richiedere e leggere informazioni senza modificarle. POST viene utilizzato per inviare nuovi dati al server e creare una nuova risorsa. PUT serve per aggiornare o sovrascrivere integralmente un dato già esistente, mentre DELETE elimina in modo permanente una risorsa specifica.

Contesto:
Sviluppo web (comunicazione tra frontend e [[backend]]), architettura del software e integrazione tra sistemi e servizi di terze parti.

Esempio:
In un'applicazione per la gestione degli utenti: usi GET per visualizzare la lista degli iscritti, POST per registrare un nuovo utente, PUT per aggiornare il profilo di un utente esistente e DELETE per cancellare il suo account.

Termine: Differenza tra GET e POST

Descrizione:
La differenza principale riguarda il modo in cui i dati vengono trasmessi e lo scopo dell'azione. GET invia eventuali parametri accodandoli direttamente all'URL (l'indirizzo web), rendendoli visibili a tutti, salvabili nei preferiti e soggetti a limiti di lunghezza; non deve mai essere usato per dati sensibili. POST invia i dati nascondendoli all'interno del "corpo" (body) della richiesta HTTP: i dati non sono visibili nell'URL, non ci sono limiti di lunghezza stringenti ed è il metodo corretto per inviare password, informazioni private o file di grandi dimensioni.

Contesto:
Sviluppo web (creazione di form, login, caricamento file) e sicurezza informatica.

Esempio:
Quando fai una ricerca su Google, stai usando una richiesta GET (puoi vedere le parole che hai cercato direttamente in alto nell'URL, ad esempio ?q=ricetta+torta). Quando accedi alla tua banca online o pubblichi una foto su Instagram, il sistema usa una richiesta POST (le tue credenziali o l'immagine viaggiano "nascoste" e non compaiono nell'indirizzo web).