---
title: metodo create_range
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 190
url: /it/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un indirizzo dell'intervallo.


###  ritorna

Un oggetto [Range](/cells/it/python-net/aspose.cells/range)


```python
def create_range(self, address):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| address | str | L'indirizzo dell'intervallo.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un intervallo di celle.


###  ritorna

Un oggetto [Range](/cells/it/python-net/aspose.cells/range)


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_cell | str | Nome della cella in alto a sinistra.|
| lower_right_cell | str | Nome della cella in basso a destra.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da righe di celle o colonne di celle.


###  ritorna

Un oggetto [Range](/cells/it/python-net/aspose.cells/range).


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| first_index | int | Indice della prima riga o indice della prima colonna, in base zero.|
| number | int | Numero totale di righe o colonne, una basata.|
| is_vertical | bool | True: intervallo creato da colonne di celle. Falso: intervallo creato da righe di celle.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Crea un oggetto [Range](/cells/it/python-net/aspose.cells/range) da un intervallo di celle.


###  ritorna

Un oggetto [Range](/cells/it/python-net/aspose.cells/range)


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| first_row | int | Prima fila di questa gamma|
| first_column | int | Prima colonna di questo intervallo|
| total_rows | int | Numero di righe|
| total_columns | int | Numero di colonne|



###  Guarda anche
* modulo [aspose.cells](../../)
* classe [Cells](/cells/it/python-net/aspose.cells/cells)
* classe [Range](/cells/it/python-net/aspose.cells/range)
