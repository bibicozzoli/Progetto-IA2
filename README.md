\# Stima della temperatura corporea tramite termografia infrarossa

\#\# Descrizione del progetto

Questo progetto di Machine Learning analizza un dataset clinico basato su \*\*misure di temperatura facciale estratte da immagini termografiche infrarosse (IRT)\*\*, con l’obiettivo di \*\*stimare la temperatura corporea orale\*\*.

Il progetto è sviluppato in Python tramite notebook Jupyter e si concentra sull’analisi dei dati, sull’addestramento di modelli di regressione e sulla valutazione delle prestazioni predittive rispetto alla temperatura orale di riferimento.

\---

\#\# Dataset

Il dataset utilizzato proviene da uno \*\*studio clinico su oltre 1000 soggetti\*\*, descritto nell’articolo:

\> Wang et al., \*Infrared Thermography for Measuring Elevated Body Temperature: Clinical Accuracy, Calibration, and Evaluation\*, Sensors, 2022\.

\#\#\# Informazioni rilevanti sul dataset

\- Per ogni soggetto sono disponibili:  
  \- una \*\*temperatura orale di riferimento\*\*, utilizzata come ground truth  
  \- diverse \*\*misure di temperatura facciale\*\* ottenute tramite immagini termografiche  
\- Le temperature facciali fanno riferimento a specifiche regioni del volto, tra cui:  
  \- fronte  
  \- fronte estesa  
  \- angolo interno dell’occhio  
  \- temperatura massima del volto  
\- Le misurazioni sono state effettuate in condizioni controllate, con l’obiettivo di valutare l’utilizzo della termografia come tecnica \*\*non invasiva\*\* per la stima della temperatura corporea

\---

\#\# Finalità dell’indagine

L’analisi ha come obiettivo principale:

\- studiare la relazione tra \*\*temperature facciali\*\* e \*\*temperatura orale\*\*  
\- valutare la possibilità di stimare la temperatura corporea a partire da misure termografiche  
\- confrontare diversi approcci di \*\*regressione\*\* in termini di accuratezza predittiva

\---

\#\# Librerie utilizzate

Il progetto è stato realizzato utilizzando le seguenti librerie:

\- \`numpy\`  
\- \`pandas\`  
\- \`matplotlib\`  
\- \`seaborn\`  
\- \`sklearn.model\_selection\`  
\- \`sklearn.decomposition\`  
\- \`sklearn.preprocessing\`  
\- \`sklearn.linear\_model\`  
\- \`sklearn.ensemble\`  
\- \`sklearn.metrics\`

\---

\#\# Analisi e metodologia 

Nel notebook \`ProgettoIA2.ipynb\` vengono eseguite le seguenti fasi:

\#\#\# 1\. Esplorazione dei dati  
\- caricamento del dataset  
\- analisi statistica delle variabili  
\- analisi dei valori mancanti

\#\#\# 2\. Preprocessing  
\- gestione dei valori mancanti  
\- selezione delle feature di input  
\- suddivisione dataset  
\- riduzione dimensionale tramite PCA  
\- gestione variabili categoriche  
\- analisi descrittiva dei set di dati finali

\#\#\# 3\. Modellazione  
\-  Scelta dei modelli di regressione: Lasso e Gradient Boosting  
\- Addestramento  
\- GroupKFold

\#\#\# 4\. Valutazione  
Le prestazioni dei modelli vengono valutate tramite:  
\- \*\*Mean Squared Error (MSE)\*\*  
\- \*\*Root Mean Squared Error (RMSE)\*\*  
\- \*\*Mean Absolute Error (MAE)\*\*

