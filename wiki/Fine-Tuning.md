Termine: Fine-Tuning (Sintonizzazione fine / Addestramento specifico)

Descrizione:
Il fine-tuning è il processo con cui si prende un modello di intelligenza artificiale già "pre-addestrato" su vaste conoscenze generali (come un [[LLM]]) e lo si sottopone a un ulteriore addestramento su un set di dati più piccolo, chiuso e altamente specifico. L'obiettivo non è insegnargli la lingua da zero, ma "plasmare" il suo comportamento per specializzarlo in un compito preciso, fargli acquisire un tono di voce aziendale, o insegnargli a produrre un formato di output molto rigido.

Contesto:
Sviluppo di AI personalizzate, Machine Learning, AI Engineering e creazione di modelli verticali (es. AI mediche o legali).

Esempio:
Prendere un modello generico e addestrarlo su 10.000 vecchi ticket di assistenza clienti della tua azienda, in modo che impari a rispondere ai futuri clienti esattamente con il tono, la cortesia e i pattern usati dai tuoi migliori operatori umani.

Differenza tra Fine-Tuning e RAG
Scegliere tra queste due tecniche è una delle decisioni architetturali più comuni e critiche quando si sviluppa un'applicazione basata sull'AI. Ecco la differenza concettuale fondamentale:

[[RAG]] (L'esame a libro aperto): Non modifica il "cervello" dell'AI. Le fornisce semplicemente una libreria di documenti aggiornati da consultare in tempo reale prima di rispondere. Se un'informazione aziendale cambia, ti basta sostituire il file nel database vettoriale e l'AI darà subito la risposta corretta.

Fine-Tuning (Lo studio a memoria): Modifica permanentemente le connessioni neurali (i "pesi") del modello. La conoscenza viene fusa direttamente nel suo cervello. È ottimo per insegnare come parlare o ragionare, ma pessimo per immagazzinare nozioni che cambiano nel tempo, perché per aggiornare un singolo fatto dovresti ripetere il costoso processo di addestramento.

Confronto Rapido

CaratteristicaRAG (Retrieval-Augmented Generation)Fine-Tuning
Scopo PrincipaleAggiungere conoscenze fattuali, dati privati o aggiornati.Insegnare un nuovo stile, formato (es. [[JSON]]), tono o abilità.
Aggiornamento DatiFacilissimo e immediato (basta aggiornare il database).Complesso e costoso (richiede un nuovo addestramento).
Costo e TempiBassi (si usano modelli standard collegati a un database).Alti (serve molta potenza di calcolo e dati preparati ad hoc).
Rischio AllucinazioniBasso (le risposte sono ancorate ai documenti forniti).Medio/Alto (il modello potrebbe confondere le nozioni memorizzate).

Per ottenere il massimo, oggi i sistemi aziendali più avanzati utilizzano un approccio ibrido: fanno un leggero fine-tuning per insegnare all'AI il gergo e il tono aziendale, e poi usano la [[RAG]] per fornirle i manuali tecnici e i dati aggiornati dei clienti.