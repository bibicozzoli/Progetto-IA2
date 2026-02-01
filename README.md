# Analisi predittiva della temperatura corporea mediante termografia facciale

Questo progetto di Machine Learning analizza due dataset clinici basati su **misure di temperatura facciale estratte da immagini termografiche infrarosse (IRT)**, con l’obiettivo di **stimare la temperatura corporea interna (orale)**.

## Dataset 1

**Nome**: FLIR_groups1and2.csv  

**Caratteristiche**: Il dataset include misurazioni termografiche facciali acquisite con una termocamera **FLIR A325sc** , temperature orali di riferimento, informazioni ambientali e dati demografici relativi a 1020 soggetti. 
- Numero campioni: 1020
- Numero features: 120
- Target: aveOralM

## Dataset 2

**Nome**: ICI_groups1and2.csv

**Caratteristiche**: Il dataset include misurazioni termografiche facciali acquisite con una termocamera **ICI 8640 P-series** , temperature orali di riferimento, informazioni ambientali e dati demografici relativi a 1009 soggetti. 
- Numero campioni: 1009
- Numero features: 120
- Target: aveOralM

## Librerie Utilizzate

- numpy
- pandas
- matplotlib
- seaborn
- scikit-learn

## Come Eseguire

1. Apri il notebook in Google Colab
2. Esegui tutte le celle

## Autori
Beatrice Cozzoli, Federico Barletta
