---
title: merge método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 790
url: /es/python-net/aspose.cells/cells/merge/
is_root: false
---
##  merge(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Combina un rango específico de celdas en una sola celda.



```python
def merge(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_row | int | Primera fila de este rango (basado en cero)|
| first_column | int | Primera columna de este rango (basado en cero)|
| total_rows | int | Número de filas (basado en uno)|
| total_columns | int | Número de columnas (basado en uno)|
###  Observaciones

Haga referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango.

##  merge(first_row, first_column, total_rows, total_columns, merge_conflict) {#int-int-int-int-bool}

Combina un rango específico de celdas en una sola celda.



```python
def merge(self, first_row, first_column, total_rows, total_columns, merge_conflict):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_row | int | Primera fila de este rango (basado en cero)|
| first_column | int | Primera columna de este rango (basado en cero)|
| total_rows | int | Número de filas (basado en uno)|
| total_columns | int | Número de columnas (basado en uno)|
| merge_conflict | bool | Combinar rangos combinados en conflicto.|
###  Observaciones

Haga referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango.
Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas,
otras celdas combinadas se eliminarán automáticamente.

##  merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict) {#int-int-int-int-bool-bool}
Combina un rango específico de celdas en una sola celda.



```python
def merge(self, first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| first_row | int | Primera fila de este rango (basado en cero)|
| first_column | int | Primera columna de este rango (basado en cero)|
| total_rows | int | Número de filas (basado en uno)|
| total_columns | int | Número de columnas (basado en uno)|
| check_conflict | bool | Indica si la verificación de las celdas combinadas se cruza con otras celdas combinadas|
| merge_conflict | bool | Combinar rangos combinados en conflicto.|
###  Observaciones

Haga referencia a la celda combinada a través de la dirección de la celda superior izquierda en el rango.
Si mergeConflict es verdadero y el rango combinado entra en conflicto con otras celdas combinadas,
otras celdas combinadas se eliminarán automáticamente.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
