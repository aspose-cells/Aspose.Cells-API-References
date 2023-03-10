---
title: metodo start_sheet
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 70
url: /it/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Inizia a salvare un foglio di lavoro.


###  ritorna

true se questo provider fornirà i dati per il foglio specificato; false se il foglio specificato deve utilizzare il suo normale modello di dati (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| sheet_index | int | indice del foglio corrente da salvare.|
###  Osservazioni

Verrà chiamato all'inizio del salvataggio di un foglio di lavoro durante il salvataggio di una cartella di lavoro.
 Se il fornitore deve fare riferimento a*`foglioIndice`* Dopo
nel metodo startRow(Row) o startCell(Cell),
 ovvero, se il processo deve sapere quale foglio di lavoro viene elaborato,
 l'implementazione dovrebbe mantenere il file*`foglioIndice`* valore qui.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/it/python-net/aspose.cells/lightcellsdataprovider)
