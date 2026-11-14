# Simulazioni Monte Carlo

Repository contenente le attività svolte durante tre giornate di laboratorio dedicate alla simulazione Monte Carlo, al fit e alla propagazione delle incertezze, a partire da un modello di frange di intensità luminosa prodotte da interferenza e diffrazione:

$$\mu(x) = B + I_0 \left[\frac{\sin(\alpha x)}{\alpha x}\right]^2 \cos^2(\delta x)$$

Ogni notebook è autonomo ed eseguibile dall'inizio alla fine. `giornata1.ipynb` genera `dati.csv`, che viene letto da `giornata2.ipynb`. Librerie utilizzate: `numpy`, `scipy`, `matplotlib`, `pandas`.

## Giornata 1 — Simulazione Monte Carlo

Dopo aver definito e rappresentato graficamente la distribuzione teorica dei conteggi, viene simulata un'acquisizione sperimentale introducendo fluttuazioni statistiche attraverso una distribuzione di Poisson.

Vengono infine generate **2000 simulazioni Monte Carlo** dell'esperimento, studiando la distribuzione del numero totale di conteggi in una regione centrale e confrontandone media e deviazione standard con i valori teorici attesi. Una delle simulazioni viene salvata in `dati.csv`.

Il codice è contenuto in `giornata1.ipynb`.

## Giornata 2 — Fit e diagnostica

Vengono analizzati i dati contenuti in `dati.csv`. Dopo una verifica preliminare, viene eseguito un **fit pesato** per stimare i parametri del modello e le relative incertezze, studiandone le correlazioni attraverso la matrice di correlazione.

La qualità del fit viene valutata tramite **residui, pull, χ² ridotto e p-value**, confrontando infine il modello completo con un modello privo dell'inviluppo per evidenziare l'importanza dei diversi termini nella descrizione dei dati.

Il codice è contenuto in `giornata2.ipynb`.

## Giornata 3 — Incertezze e covarianze

A partire dai parametri del fit $(\alpha, \delta)$ e dalla loro covarianza, insieme a due fattori di calibrazione $(k, s_x)$, vengono propagate le incertezze alle grandezze derivate $a$, $d$ e $q = d/a$.

Il calcolo **analitico** (Jacobiano) viene confrontato con un **Monte Carlo correlato**; si studia poi l'effetto di ignorare le correlazioni, si ricava la **mappa dei contributi** di ogni sorgente e si confrontano alcuni scenari di miglioramento (statistica del fit, calibrazioni).

Il codice è contenuto in `giornata3.ipynb`.

## Collaboratori

- Tommaso Malaguti
- Davide Patarchi
- Leonardo Patricolo
- Linda Spadoni
