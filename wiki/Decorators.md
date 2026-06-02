Termine: Decorator (Decoratore)

Descrizione:
Un decorator è una funzione in [[Python]] che prende un'altra funzione (o [[classe]]) e ne estende o modifica il comportamento senza alterarne il codice sorgente interno. Agisce come un "involucro" (wrapper) che può eseguire istruzioni aggiuntive prima o dopo l'esecuzione della funzione originale. Si applica in modo semplice ed elegante scrivendo il simbolo @ seguito dal nome del decoratore direttamente sopra la definizione della funzione interessata.

Contesto:
Sviluppo software, [[Python]], riutilizzo del codice (spesso usati per creare log, gestire autorizzazioni, misurare i tempi di esecuzione o gestire la cache).

Esempio:
Se scrivi un decoratore @richiede_login sopra la funzione visualizza_messaggi_privati(), il sistema verificherà automaticamente che l'utente sia autenticato prima di fargli leggere i messaggi, bloccandolo in caso contrario.

Termine: @classmethod e @staticmethod

Descrizione:
Sono due decoratori predefiniti di [[Python]] utilizzati per modificare il comportamento dei metodi all'interno di una [[classe]]. Il @classmethod fa sì che il metodo riceva come primo parametro la [[classe]] stessa (convenzionalmente chiamata cls) invece dell'[[istanza]] dell'oggetto, permettendo di manipolare lo stato generale della [[classe]]. Il @staticmethod, invece, "scollega" il metodo sia dall'[[istanza]] che dalla [[classe]]: il metodo non riceverà alcun parametro nascosto e si comporterà come una normale funzione, ma resterà logicamente raggruppato all'interno della [[classe]] per questioni di ordine.

Contesto:
Programmazione Orientata agli Oggetti ([[OOP]]) e architettura del codice in [[Python]].

Esempio:
Usa un @classmethod per creare costruttori alternativi, come Documento.crea_da_pdf(), che genera e restituisce un nuovo oggetto partendo da un file. Usa un @staticmethod per funzioni di utilità pura che non hanno bisogno di leggere i dati dell'oggetto, come Documento.verifica_formato_data("2023-10-12").