# Customer Churn Prediction — Progetto Data Science (Gruppo 8)
Questo è un progetto per il corso di *Introduzione alla Data Science e al pensiero computazionale* (a.a. 2025-26). 
L'obiettivo è prevedere se un cliente di un'azienda di telecomunicazioni abbandonerà il servizio (*Churn*), a partire da informazioni demografiche, contrattuali e di utilizzo.

## Obiettivo
Costruire e confrontare modelli di classificazione binaria in grado di prevedere la variabile `Churn` (Yes/No), individuando i principali fattori associati all'abbandono dei clienti.

## Dataset
- **Fonte:** Telco Customer Churn
- **Osservazioni:** 7.043 clienti
- **Variabili:** 21 (demografiche, di servizio, contrattuali e di spesa)
- **Variabile target:** `Churn` (Yes/No), con distribuzione squilibrata (~73,5% No / ~26,5% Yes)

## Struttura del repository
/
├──DATA/
├──Notebook/
├──FIGURES/
├──REPORT/
├── README.md

## Fasi del progetto
1. **Descrizione e Comprensione del dataset** — analisi di dimensioni, tipi di variabili, valori mancanti e distribuzione della variabile target.
2. **Analisi esplorativa e visualizzazione** — studio delle relazioni tra le variabili e il churn (tipo di contratto, anzianità, spesa, servizio internet, ecc.).
3. **Modellazione** — codifica delle variabili categoriche, gestione dei valori mancanti, suddivisione Train/Test 70/30 stratificata e addestramento di tre modelli di classificazione:
    - Decision Tree
    - Regressione Logistica
    - Random Forest
4. **Valutazione e interpretazione** — confronto dei modelli tramite metriche di classificazione (accuracy, precision, recall, F1) e interpretazione dei risultati.

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
