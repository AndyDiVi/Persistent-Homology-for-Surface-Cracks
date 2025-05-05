# 🔍 Persistent Homology for Surface Cracks Classification - Bachelor Thesis

🎓 Tesi Triennale presso l'università di Genova, premiata con il “Matteo Dellepiane Award” per la miglior tesi triennale in Computer Graphics – 2024.

La tesi esplora l'applicazione dell'omologia persistente nella classificazione di immagini di superfici crepate. Dopo un'introduzione teorica ai concetti topologici fondamentali (complessi simpliciali, omologia simpliciale e singolare), si passa all'analisi pratica tramite costruzione di filtrazioni, in particolare con il complesso di Vietoris-Rips. Le immagini vengono preprocessate (binarizzazione e padding) e analizzate con tecniche di data analysis topologica. I risultati, valutati tramite matrice di confusione, mostrano che l'omologia persistente supera, in questo contesto, metodi tradizionali come SVM e Random Forest.

![Strategia usata](strategy.png)

##Abstract 
Questa tesi esplora la nozione di omologia persistente, un potente strumento dell'analisi topologica dei dati, con particolare attenzione alla sua applicazione nella classificazione di immagini di superfici crepate. Si inizia definendo concetti base come complessi simpliciali, complessi delta e l'omologia simpliciale. In particolare, viene costruito un ponte tra l'omologia singolare e l'omologia simpliciale, rivelando l'intercambiabilità delle conoscenze tra i due domini.
Lo studio progredisce fino a definire l'omologia persistente e la nozione essenziale di filtrazione. Si illustrano vari metodi di costruzione di filtrazioni da insiemi di dati, enfatizzando il complesso di Čech e il complesso di Vietoris-Rips. Quest'ultimo, applicato alle immagini di superfici crepate, opportunamente elaborate attraverso la binarizzazione e l'aggiunta di un bordo, svela un nuovo approccio al rilevamento delle crepe. Il primo gruppo di omologia persistente diventa una metrica chiave, rappresentando il numero di buchi nel complesso e servendo come caratteristica distintiva per la classificazione delle crepe. Si presentano esempio pratici e i relativi diagrammi di persistenza per evidenziare i punti di forza e i limiti del metodo.
 Il culmine è rappresentato dalla creazione di una matrice di confusione, fornendo una valutazione completa dell'accuratezza predittiva del modello rispetto alla verità. 
Infine, viene condotta un'analisi comparativa con gli algoritmi tradizionali di apprendimento automatico, in particolare con le macchine a supporto vettoriale (SVM) e le foreste casuali. Sorprendentemente, l'omologia persistente emerge come strumento più efficace per la classificazione della superficie delle crepe, dimostrando la sua superiorità rispetto ai metodi convenzionali. Questo studio contribuisce non solo alla comprensione teorica dell'omologia persistente, ma mostra anche la sua abilità pratica nelle applicazioni del mondo reale, in particolare nella classificazione d'immagini.

# Getting Started
## 🗂 Contenuto del Repository

- `Binarize.ipynb` – Notebook per le diverse tecniche di binarizzazione esplorate e preparazione delle immagini
- `Project.ipynb` – Notebook principale per pre-processing, analisi topologica, classificazione e confronto
- `requirements.txt` – Librerie necessarie per l'esecuzione
- `DiVia_Andrea_tesi.pdf` – Tesi di laurea per intero
- `DiVia_Andrea_tesi_ppt.pdf` – Slide per la presentazione della tesi di laurea
- `README.md` – Questo file
  
## Installation
Install python packages
```
pip install -r requirements.txt
```

## Preparing Datasets
Download the [cracks](https://www.kaggle.com/datasets/arunrk7/surface-crack-detection) dataset and prepare the following directory structure.
    - Cracks
        -  Negative
            - Negative_00001.jpg
            ...
            - Negative_20000.jpg
        -  Positive
            - Positive_00001.jpg
            ...
            - Positive_20000.jpg
         

## Running Experiments
To run the experiments, follow these steps:
```
`Project.ipynb`
```
