# Customer Churn Prediction — Progetto Data Science (Gruppo 8)
Questo è un progetto per il corso di *Introduzione alla Data Science e al pensiero computazionale* (a.a. 2025-26). 
L'obiettivo è prevedere se un cliente di un'azienda di telecomunicazioni abbandonerà il servizio (*Churn*), a partire da informazioni demografiche, contrattuali e di utilizzo.

## Obiettivo
Costruire e confrontare modelli di classificazione binaria in grado di prevedere la variabile `Churn` (Yes/No), individuando i principali fattori associati all'abbandono dei clienti.

## Dataset
- **Fonte:** Telco Customer Churn
- **Osservazioni:** 7043 clienti
- **Variabili:** 21 (demografiche, di servizio, contrattuali e di spesa)
- **Variabile target:** `Churn` (Yes/No), con distribuzione squilibrata (~73.5% No / ~26.5% Yes)

## Struttura del repository
```
/
├── DATA/
├── FIGURES/
├── Notebook/
├── REPORT/
├── LICENSE
└── README.md
```


## Fasi del progetto
Nel Notebook del progetto sono contenute le seguenti fasi: 

1. **Descrizione e Comprensione del dataset** — analisi di dimensioni, tipi di variabili, valori mancanti, distribuzione della variabile target 'Churn', delle variabili di spesa, dei servizi di rete e di intrattenimento, del metodo di pagamento e del tipo di contratto .
2. **Analisi esplorativa e visualizzazione** — studio delle relazioni tra le variabili e il churn (tipo di contratto, anzianità, spesa, servizio internet, ecc.).
3. **Modellazione** — codifica delle variabili categoriche, gestione dei valori mancanti, eliminazione della variabile Customer ID, suddivisione Train/Test 70/30 stratificata e addestramento di tre modelli di classificazione:
    - Decision Tree
    - Regressione Logistica
    - Random Forest

A partire dalla feature importance della Random Forest, è stato selezionato un sottoinsieme di 6 variabili che maggiormente influiscono sulla variabile 'Churn', sulla base delle quali sono stati nuovamente addestrati i modelli. 

Per ciascun modello sono state calcolate le metriche di classificazione (accuracy, precision, recall, F1) e la relativa matrice di confusione.

4. **Valutazione e interpretazione dei risultati** — confronto dei modelli tramite le metriche di classificazione precedentemente misurate e interpretazione dei risultati.

## Report
Il progetto include un **report**, redatto in LaTeX tramite Overleaf, che accompagna e completa l'analisi. Mentre il notebook documenta passo passo il codice e i risultati, il report è il luogo in cui questi risultati vengono **interpretati e discussi**

Il report è organizzato nelle seguenti sezioni:

- **Introduzione** — Descrizione dell'obiettivo del progetto: prevedere l'abbandono di un cliente (`Churn`, Yes/No) a partire da variabili demografiche, contrattuali e di servizio.
- **Descrizione del dataset** — Struttura del dataset Telco Customer Churn, distribuzione del target e analisi della qualità dei dati.
- **Metodologia** — La metodologia contiene inormazioni riguardo l'analisi esplorativa (descrizione delle ipotesi formulate e profilo del cliente a rischio abbandono) e la fase di modellazione (preprocessing, codifica delle variabili, suddivisione Train/Test e scelta dei tre modelli).
- **Risultati** — Le metriche di ciascun modello (accuracy, precision, recall, F1) raccolte in una tabella comparativa.
- **Discussione** — Punti di forza e limiti di ciascun modello, tipologia di errori, interpretabilità e costo computazionale dei tre approcci. I risultati vengono infine ricollegati alle ipotesi formulate nella fase esplorativa.
- **Conclusione** — Sintesi dei risultati.

## Librerie Python utilizzate
- Pandas, NumPy
- Matplotlib, Seaborn
- Scikit-learn

## Come eseguire
Il notebook è stato sviluppato in Google Colab. Per eseguirlo:
1. Aprire `ProgettoDataScienceGruppo_8.ipynb` in Google Colab.
2. Caricare il file `Customer_Churn.csv`.
3. Eseguire le celle in ordine.

## Autori — Gruppo 8
- Gaia Gasparini
- Aurora Paolicchi
- Lucrezia Volpato
