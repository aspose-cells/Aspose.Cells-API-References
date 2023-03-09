---
title: pivot_source proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 400
url: /it/python-net/aspose.cells.charts/chart/pivot_source/
is_root: false
---
##  pivot_source proprietà

La fonte sono i dati della tabella pivot.
Se PivotSource non è vuoto, il grafico è PivotChart.

###  Osservazioni

Se la tabella pivot "PivotTable1" nel foglio di lavoro "Sheet1" nel file "Book1.xls".
Il pivotSource potrebbe essere "[Book1.xls]Sheet1!PivotTable1" se il grafico e la tabella pivot non si trovano nella stessa cartella di lavoro.
Se imposti questa proprietà, l'impostazione dell'origine dati precedente andrà persa.
###  Definizione:
```python
@property
def pivot_source(self):
    ...
@pivot_source.setter
def pivot_source(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [Chart](/cells/it/python-net/aspose.cells.charts/chart)
