Termine: Programmazione Asincrona (async / asyncio)

Descrizione:
L'asincronia è un modello di programmazione che permette a un programma di avviare un'operazione lunga e, anziché bloccarsi in attesa che finisca, continuare a eseguire altre attività nel frattempo. In [[Python]], il modulo asyncio e le parole chiave async/await gestiscono questo processo, mettendo in pausa una funzione quando deve aspettare un risultato esterno e riprendendola appena il dato è pronto. Questo approccio ottimizza enormemente i tempi morti sfruttando un singolo processo (thread), rendendo il software molto più veloce ed efficiente nella gestione delle attese.

Contesto:
Sviluppo web (es. framework come [[FastAPI]]), web scraping, bot per chat (Telegram, Discord) e operazioni "I/O bound" (lettura/scrittura su disco o richieste di rete).

Esempio:
Useresti asyncio per creare un programma che deve scaricare dati da 100 siti web diversi: anziché scaricare una pagina alla volta aspettando passivamente la risposta di ogni singolo server, il codice asincrono lancia tutte le richieste quasi simultaneamente ed elabora i dati man mano che ogni server risponde, riducendo drasticamente il tempo totale di esecuzione.