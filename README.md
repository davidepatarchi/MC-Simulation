# Simulazioni Monte Carlo

Repository contenente le attività svolte durante due giornate di laboratorio dedicate alla simulazione Monte Carlo e all'analisi statistica dei dati.

## Giornata 1 — Simulazione Monte Carlo

Nella prima giornata viene studiato un modello di frange di intensità luminosa prodotte da interferenza e diffrazione.

Dopo aver definito e rappresentato graficamente la distribuzione teorica dei conteggi, viene simulata un'acquisizione sperimentale introducendo fluttuazioni statistiche attraverso una distribuzione di Poisson.

Vengono infine generate **2000 simulazioni Monte Carlo** dell'esperimento, studiando la distribuzione del numero totale di conteggi in una regione centrale e confrontandone media e deviazione standard con i valori teorici attesi.

Il codice è contenuto in `giornata1.ipynb`.

## Giornata 2 — Fit e analisi statistica

Nella seconda giornata vengono analizzati i dati contenuti in `dati.csv`.

Dopo una verifica preliminare dei dati, viene eseguito un **fit del modello teorico** per stimarne i parametri e le relative incertezze. Vengono inoltre studiate le correlazioni tra i parametri attraverso la matrice di correlazione.

La qualità del fit viene valutata tramite **residui, pull, χ² ridotto e p-value**, confrontando infine il modello completo con un modello semplificato per evidenziare l'importanza dei diversi termini nella descrizione dei dati.

Il codice è contenuto in `giornata2.ipynb`.

## Collaboratori

- Tommaso Malaguti
- Patarchi Davide
- Patricolo Leonardo
- Spadoni Linda