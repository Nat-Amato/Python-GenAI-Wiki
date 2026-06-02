Termine: List Comprehension (Comprensione di liste)

Descrizione:
La list comprehension è un costrutto sintattico avanzato di [[Python]] che permette di creare nuove liste in modo rapido e conciso, racchiudendo l'intera operazione in un'unica riga di codice. Invece di utilizzare un tradizionale ciclo for distribuito su più righe, si definisce l'elemento da generare, il ciclo su cui iterare e le eventuali condizioni di filtro, tutto all'interno di parentesi quadre. Questo rende il codice più compatto, leggibile e spesso più veloce nell'esecuzione.

Contesto:
Sviluppo software, scripting in [[Python]] e ottimizzazione del codice.

Esempio:
Scrivendo numeri = [x*x for x in range(10)], ottieni istantaneamente una lista contenente i quadrati dei numeri da 0 a 9 [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]. Questo sostituisce la necessità di creare una lista vuota e riempirla gradualmente con un ciclo for e il comando append().