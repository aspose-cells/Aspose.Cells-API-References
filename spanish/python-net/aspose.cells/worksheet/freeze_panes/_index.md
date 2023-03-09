---
title: freeze_panes método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 120
url: /es/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
Congela los paneles en la celda especificada de la hoja de cálculo.



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell_name | str | Cell nombre.|
| freezed_rows | int | Número de filas visibles en el panel superior, no más que el índice de fila.|
| freezed_columns | int | Número de columnas visibles en el panel izquierdo, no más que el índice de columna.|
###  Observaciones

El índice de fila y el índice de columna no pueden ser todos cero.
tampoco puede ser todo cero.

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
Congela los paneles en la celda especificada de la hoja de cálculo.



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| row | int | Índice de fila.|
| column | int | Índice de columnas.|
| freezed_rows | int | Número de filas visibles en el panel superior, no más que el índice de fila.|
| freezed_columns | int | Número de columnas visibles en el panel izquierdo, no más que el índice de columna.|
###  Observaciones

El índice de fila y el índice de columna no pueden ser todos cero.
tampoco puede ser todo cero.


Los dos primeros parámetros especifican la posición congelada y los dos últimos parámetros especifican el área congelada en el panel superior izquierdo.


###  Ver también
* módulo [aspose.cells](../../)
* clase [Worksheet](/cells/es/python-net/aspose.cells/worksheet)
