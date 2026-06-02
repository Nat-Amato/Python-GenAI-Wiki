Termine: Vector Database (Database Vettoriale)

Descrizione:
Un database vettoriale è progettato specificamente per memorizzare, gestire e cercare dati che sono stati trasformati in [[embedding]] (lunghe sequenze di numeri o vettori). La necessità di questi database nasce da un limite fondamentale dei database tradizionali (come quelli SQL): i sistemi classici trovano le informazioni cercando corrispondenze esatte di parole chiave o filtri rigidi. Un database vettoriale, al contrario, esegue ricerche basate sul significato e sul contesto (ricerca semantica).

Poiché i concetti con significati simili vengono convertiti in vettori con coordinate matematicamente vicine, il database vettoriale calcola la "distanza" tra la domanda dell'utente e i dati archiviati. Questo permette alle intelligenze artificiali di frugare in millisecondi tra milioni di documenti non strutturati (testi, PDF, immagini, audio) e recuperare le informazioni concettualmente più pertinenti per rispondere.

Contesto:
Intelligenza Artificiale Generativa, architetture [[RAG]] (Retrieval-Augmented Generation), motori di ricerca semantica, sistemi di raccomandazione e analisi di dati non strutturati.

Esempio:
Se cerchi "cucciolo fedele" nel database del tuo sito, un database tradizionale (basato su parole chiave) non troverà mai un articolo intitolato "giovane cane leale", perché le parole esatte non combaciano. Un database vettoriale (come Pinecone o Milvus), invece, capirà immediatamente che i due concetti si trovano nella stessa area matematica dello spazio vettoriale e ti restituirà l'articolo corretto.