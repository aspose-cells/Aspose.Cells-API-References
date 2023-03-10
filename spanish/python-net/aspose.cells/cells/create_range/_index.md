---
title: create_range método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 190
url: /es/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de una dirección del rango.


###  Devoluciones

Un objeto [Range](/cells/es/python-net/aspose.cells/range)


```python
def create_range(self, address):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| address | str | La dirección del rango.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de un rango de celdas.


###  Devoluciones

Un objeto [Range](/cells/es/python-net/aspose.cells/range)


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| upper_left_cell | str | Nombre de la celda superior izquierda.|
| lower_right_cell | str | Nombre de la celda inferior derecha.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de filas de celdas o columnas de celdas.


###  Devoluciones

Un objeto [Range](/cells/es/python-net/aspose.cells/range).


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_index | int | Índice de la primera fila o índice de la primera columna, basado en cero.|
| number | int | Número total de filas o columnas, basado en uno.|
| is_vertical | bool | Verdadero: rango creado a partir de columnas de celdas. Falso: rango creado a partir de filas de celdas.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Crea un objeto [Range](/cells/es/python-net/aspose.cells/range) a partir de un rango de celdas.


###  Devoluciones

Un objeto [Range](/cells/es/python-net/aspose.cells/range)


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_row | int | Primera fila de este rango|
| first_column | int | Primera columna de este rango|
| total_rows | int | Número de filas|
| total_columns | int | Número de columnas|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
* clase [Range](/cells/es/python-net/aspose.cells/range)
