Termine: Data Leakage (Fuga o Dispersione di Dati) nell'AI

Descrizione:
Il Data Leakage si verifica quando informazioni sensibili, private o segrete vengono esposte in modo non autorizzato a causa di un uso scorretto o di una configurazione errata dei sistemi AI. Quando si sviluppano applicazioni GenAI, i rischi di dispersione si concentrano principalmente su tre fronti, che richiedono protezioni specifiche:

Dati Aziendali (Proprietà Intellettuale): Avviene spesso quando i dipendenti incollano codice sorgente segreto, strategie finanziarie o documenti riservati in modelli [[LLM]] pubblici (come la versione base di ChatGPT) per farsi fare dei riassunti.

Protezione: Utilizzare versioni Enterprise o istanze private dei modelli AI, che garantiscono contrattualmente che i dati inviati non verranno mai utilizzati per addestrare i modelli pubblici dell'azienda fornitrice.

Dati dei Clienti (Privacy e GDPR): Se un sistema [[RAG]] (Retrieval-Augmented Generation) è configurato male, potrebbe usare i documenti medici o bancari dell'Utente A per rispondere a una domanda posta dall'Utente B.

Protezione: Implementare rigidi controlli di accesso (RBAC - Role-Based Access Control) direttamente nel [[Vector Database]]. L'AI deve poter "pescare" solo i documenti che l'utente che sta facendo la domanda ha il permesso di leggere. Tecniche di anonimizzazione dei dati prima dell'invio all'[[LLM]] sono altrettanto fondamentali.

[[API]] Key (Chiavi di Accesso): Il rischio più da principianti ma fatale. Consiste nello scrivere in chiaro le password del database o la chiave segreta (es. la propria OpenAI [[API]] Key) direttamente nel codice sorgente o all'interno del [[prompt]] inviato al modello.

Protezione: Non scrivere mai le chiavi nel codice. Vanno salvate in variabili d'ambiente (file .env esclusi dal controllo versione come Git) o gestite tramite servizi sicuri di Secret Management (come AWS Secrets Manager o Azure Key Vault).

Contesto:
Conformità legale (GDPR, HIPAA), architettura software sicura, DevSecOps e gestione delle identità e degli accessi (IAM).