# Struttura di un esame

In seguito sono descritti i vari componenti che formano un esame.

## Nome, data e ora di inizio e di fine

Ogni esame deve avere un nome, una data e ora di inizio e una data e ora di fine. L'esame inizia automaticamente alla data e ora di inizio, ma 
*non* termina in maniera automatica: è quindi compito del docente *chiudere* l'esame.

## Codice accesso

Ogni esame ha associato un codice di accesso univoco, che viene generato in automatico dopo la creazione dell'esame. Questo codice deve essere comunicato agli studenti per poterli fare partecipare all'esame.

## Domande teoriche, esercizi di programmazione e categorie

Un esame è formato da una serie di ***domande teoriche*** e ***esercizi di programmazione***. Ciascuna domanda  fa parte di una ***categoria di domande***. Analogamente, ciascun esercizio fa parte di una ***categoria di esercizi di programmazione***.

In generale, una ***categoria*** raggruppa un sottoinsieme di domande o esercizi che sono considerate simili o che trattano lo stesso argomento. Ecco alcuni esempi di possibili categorie:

* *Domande su P e NP*.

* *Domande sul Master Theorem*.

* *Esercizi di programmazione su grafi*.

### Domande teoriche
Esistono due tipologie di domande teoriche:

*  ***Domanda aperte***: lo studente potrà rispondere liberamente alla domanda.
* ***Domande a scelta multipla***: lo studente per rispondere ad una domanda potrà selezionare una o più risposte da un insieme predefinito di risposte possibili definito dal docente.

### Categoria di domande teoriche

Una ***categoria di domande teoriche*** è caratterizzata da:

* Il *nome della categoria*.
* Se la categoria deve essere è *randomizzata* oppure no:
	* ***Se la randomizzata è attiva***, si deve specificare Il *numero di domande della categoria che devono essere mostrate agli studenti durante l'esame*. Inserendo un numero minore del numero effettivo di domande della categoria, durante l'esame ad ogni studente verrà mostrato un sottoinsieme di domande scelte *casualmente* tra quelle della categoria.
	* ***Se la randomizzazione non è attiva***, durante l'esame ad ogni studente verranno mostrate tutte le domande di questa categoria, nell'ordine con cui sono state inserite.
* Se la categoria deve essere usata come ***domanda aggregata***. Una domanda aggregata è un insieme di domande che condividono una introduzione comune.  Ad esempio, potrei avere come introduzione un immagine di un grafo e poi delle domande relative al grafo dell'immagine.

### Esercizi di programmazione
Un esercizio di programmazione è formato da:

* Il testo dell'esercizio.
* Del codice iniziale, opzionale, fornito dal docente agli studenti.
* Un insieme di ***testcase*** con cui gli studenti possono testare la correttezza del loro programmi.
* Il numero minimo di testcase che il programma dello studente deve superare per poter essere consegnato.

### Testcase
I testcase devono essere scritti utilizzando il modulo [assert](https://nodejs.org/api/assert.html) di NodeJS. Esistono due tipologie di testcase:

* ***Testcase pubblici***: sono visualizzabili dagli studenti.
* ***Testcase segreti***: sono visualizzabili solamente dai docenti e non dagli studenti.
### Categoria di esercizi di programmazione

Una ***categoria di esercizi di programmazione*** è caratterizzata da:

* Il *nome della categoria*.
* Se la categoria deve essere è *randomizzata* oppure no:
	* ***Se la randomizzata è attiva***, si deve specificare Il *numero di esercizi di programmazione della categoria che devono essere mostrate agli studenti durante l'esame*. Inserendo un numero minore del numero effettivo di esercizi della categoria, durante l'esame ad ogni studente verrà mostrato un sottoinsieme di esercizi di programmazione scelte *casualmente* tra quelle della categoria.
	* ***Se la randomizzazione non è attiva***, durante l'esame ad ogni studente verranno mostrate tutte gli esercizi di programmazione di questa categoria, nell'ordine con cui sono stati inseriti.


## Docenti referenti

È possibile aggiungere dei docenti referenti ad un esame. In generale, i docenti referenti hanno le stesse capacità del creatore dell'esame. 
Ad esempio, i docenti referenti possono accedere all'esame e modificarlo, monitorare l'esame, chiudere le
consegne una volta iniziato l'esame e scaricare gli esami degli studenti che hanno partecipato all'esame.
