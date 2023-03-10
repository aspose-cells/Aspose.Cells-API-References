---
title: calculation_id proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 50
url: /it/python-net/aspose.cells/formulasettings/calculation_id/
is_root: false
---
##  calculation_id proprietà

Specifica la versione del motore di calcolo utilizzato per calcolare i valori nella cartella di lavoro.

###  Osservazioni

Questa proprietà serve solo per salvare le impostazioni nel file del foglio di calcolo risultante
in modo che altre applicazioni (come ms excel) possano agire di conseguenza durante il caricamento e la manipolazione del file risultante.
Nel caso di ms excel, se il valore di questa proprietà è minore dell'identificativo del motore di ricalcolo associato
con l'applicazione che apre il file risultante, l'applicazione ricalcolerà i risultati di tutte le formule
su questa cartella di lavoro subito dopo aver caricato il file.
Per considerazione delle prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula sulla cartella di lavoro,
indipendentemente dal valore impostato per questa proprietà.
###  Definizione:
```python
@property
def calculation_id(self):
    ...
@calculation_id.setter
def calculation_id(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [FormulaSettings](/cells/it/python-net/aspose.cells/formulasettings)
