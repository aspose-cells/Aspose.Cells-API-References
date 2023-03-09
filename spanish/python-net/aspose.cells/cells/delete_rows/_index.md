---
title: delete_rows método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 260
url: /es/python-net/aspose.cells/cells/delete_rows/
is_root: false
---
##  delete_rows(row_index, total_rows) {#int-int}
Elimina varias filas.



```python
def delete_rows(self, row_index, total_rows):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| row_index | int | El índice de la primera fila que se eliminará.|
| total_rows | int | Número de filas a eliminar.|
###  Observaciones

Si el rango eliminado contiene la parte superior (no todo) de la tabla (ListObject),
el rango no se pudo eliminar y no se hará nada. Funciona como MS Excel.

##  delete_rows(row_index, total_rows, update_reference) {#int-int-bool}
Elimina varias filas en la hoja de cálculo.


###  Devoluciones




```python
def delete_rows(self, row_index, total_rows, update_reference):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| row_index | int | Índice de fila.|
| total_rows | int | Número de filas a eliminar.|
| update_reference | bool | Indica si actualizar referencias en otras hojas de cálculo.|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Cells](/cells/es/python-net/aspose.cells/cells)
