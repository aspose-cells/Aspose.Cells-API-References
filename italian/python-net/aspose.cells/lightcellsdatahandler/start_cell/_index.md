---
title: metodo start_cell
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 40
url: /it/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Si prepara a processare una cella.


###  ritorna

se questa cella deve essere elaborata. false per ignorare la cella e controllare quella successiva fino a raggiungere la fine dei dati della cella della riga corrente


```python
def start_cell(self, column_index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| column_index | int | indice di colonna della cella da elaborare|
###  Osservazioni

Verrà chiamato quando si raggiunge una cella esistente nella riga corrente. La riga corrente è la riga dell'ultima chiamata di [LightCellsDataHandler.process_row(row)](/cells/it/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Guarda anche

* modulo [aspose.cells](../../)
* classe [LightCellsDataHandler](/cells/it/python-net/aspose.cells/lightcellsdatahandler)
