---
title: metodo add
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 20
url: /it/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Aggiunge un grafico alla raccolta.


###  ritorna

[Chart](/cells/it/python-net/aspose.cells.charts/chart) indice oggetto.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [ChartType](/cells/it/python-net/aspose.cells.charts/charttype) | Tipo di grafico|
| upper_left_row | int | Indice della riga in alto a sinistra.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| lower_right_row | int | Indice riga in basso a destra|
| lower_right_column | int | Indice colonna in basso a destra|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Aggiunge un grafico alla raccolta.


###  ritorna

[Chart](/cells/it/python-net/aspose.cells.charts/chart) indice oggetto.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [ChartType](/cells/it/python-net/aspose.cells.charts/charttype) | Tipo di grafico|
| data_range | str | Specifica l'intervallo di dati del grafico|
| top_row | int | Indice della riga in alto a sinistra.|
| left_column | int | Indice colonna in alto a sinistra.|
| right_row | int | Indice riga in basso a destra|
| bottom_column | int | Indice colonna in basso a destra|
###  Osservazioni

NOTA: questo membro è ora obsoleto. Invece,
si prega di utilizzare la proprietà [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/it/python-net/aspose.cells.charts/chartcollection/add).
 Questa proprietà verrà rimossa 12 mesi dopo da maggio 2022.
Aspose si scusa per gli eventuali disagi causati.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Aggiunge un grafico con modello preimpostato.


###  ritorna

[Chart](/cells/it/python-net/aspose.cells.charts/chart) indice oggetto.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| data | bytes | I dati del file modello grafico (.crtx).|
| data_range | str | Specifica l'intervallo di dati del grafico|
| is_vertical | bool | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna.|
| top_row | int | Indice della riga in alto a sinistra.|
| left_column | int | Indice colonna in alto a sinistra.|
| right_row | int | Indice riga in basso a destra|
| bottom_column | int | Indice colonna in basso a destra|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Aggiunge un grafico alla raccolta.


###  ritorna

[Chart](/cells/it/python-net/aspose.cells.charts/chart) indice oggetto.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [ChartType](/cells/it/python-net/aspose.cells.charts/charttype) | Tipo di grafico|
| data_range | str | Specifica l'intervallo di dati del grafico|
| is_vertical | bool | Specifica se tracciare la serie da un intervallo di valori di cella per riga o per colonna.|
| top_row | int | Indice della riga in alto a sinistra.|
| left_column | int | Indice colonna in alto a sinistra.|
| right_row | int | Indice riga in basso a destra|
| bottom_column | int | Indice colonna in basso a destra|



###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [Chart](/cells/it/python-net/aspose.cells.charts/chart)
* classe [ChartCollection](/cells/it/python-net/aspose.cells.charts/chartcollection)
