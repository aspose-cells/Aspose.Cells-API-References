---
title: metodo start_row
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 60
url: /it/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Inizia a salvare i dati di una riga.



```python
def start_row(self, row):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| row | [Row](/cells/it/python-net/aspose.cells/row) | Oggetto riga per l'implementazione per riempire i dati. Il relativo indice di riga è il valore restituito dell'ultima chiamata di [LightCellsDataProvider.next_row()](/cells/it/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Se la riga è stata inizializzata nel modello di celle interne, verrà utilizzato l'oggetto riga esistente.<br/> In caso contrario, verrà utilizzato un oggetto Row temporaneo per l'implementazione per riempire i dati.|
###  Osservazioni

Verrà chiamato all'inizio del salvataggio di una riga e dei dati delle sue celle.
Se la riga corrente ha alcune proprietà personalizzate come altezza, stile, ...ecc.,
l'implementazione dovrebbe impostare queste proprietà sull'oggetto Row specificato qui.


###  Guarda anche
* modulo [aspose.cells](../../)
* classe [LightCellsDataProvider](/cells/it/python-net/aspose.cells/lightcellsdataprovider)
