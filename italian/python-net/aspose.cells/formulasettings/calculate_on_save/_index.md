---
title: calculate_on_save proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/formulasettings/calculate_on_save/
is_root: false
---
##  calculate_on_save proprietà

Indica se ricalcolare la cartella di lavoro prima di salvare il documento, in modalità di calcolo manuale.

###  Osservazioni

Questa proprietà serve solo per salvare le impostazioni nel file del foglio di calcolo risultante
in modo che altre applicazioni (come ms excel) possano agire di conseguenza durante il caricamento e la manipolazione del file risultante.
Per considerazioni sulle prestazioni per la maggior parte delle applicazioni degli utenti, non calcoliamo automaticamente alcuna formula nella cartella di lavoro,
indipendentemente dal valore impostato per questa proprietà.
###  Definizione:
```python
@property
def calculate_on_save(self):
    ...
@calculate_on_save.setter
def calculate_on_save(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [FormulaSettings](/cells/it/python-net/aspose.cells/formulasettings)
