---
title: metodo process_row
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 30
url: /it/python-net/aspose.cells/lightcellsdatahandler/process_row/
is_root: false
---
##  process_row(row) {#Row}
Inizia a elaborare una riga.


###  ritorna

se le celle di questa riga devono essere elaborate. false per ignorare tutte le celle in questa riga.


```python
def process_row(self, row):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| row | [Row](/cells/it/python-net/aspose.cells/row) | Oggetto riga attualmente in fase di elaborazione.|
###  Osservazioni

Sarà chiamato dopo le proprietà della riga come altezza, stile, ... ecc. sono stati letti. Tuttavia, le celle in questa riga non sono state ancora lette.


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/it/python-net/aspose.cells/lightcellsdatahandler)
