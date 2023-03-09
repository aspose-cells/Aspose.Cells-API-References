---
title: trim_leading_blank_row_and_column proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 220
url: /it/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column proprietà

Indica se le righe e le colonne vuote iniziali devono essere tagliate come fa ms excel.
L'impostazione predefinita è true.

###  Osservazioni

Lo stesso con la regola in ms excel, una riga/colonna non verrà considerata vuota se ha uno stile personalizzato,
anche se non contiene dati di cella.
Quando si salva con la modalità LightCells, questa opzione non ha effetto.
L'utente deve controllare l'intervallo di output mediante l'implementazione di [TxtSaveOptions.light_cells_data_provider](/cells/it/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
oppure parlando allo [TxtSaveOptions.export_area](/cells/it/python-net/aspose.cells/txtsaveoptions#export_area)
###  Definizione:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells](../../)
* classe [TxtSaveOptions](/cells/it/python-net/aspose.cells/txtsaveoptions)
