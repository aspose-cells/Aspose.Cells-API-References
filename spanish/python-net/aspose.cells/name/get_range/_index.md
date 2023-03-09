---
title: get_range método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/name/get_range/
is_root: false
---
##  get_range() {#}
Obtiene el rango si este nombre hace referencia a un rango.


###  Devoluciones

El rango.


```python
def get_range(self):
    ...
```




##  get_range(recalculate) {#bool}
Obtiene el rango si este nombre hace referencia a un rango


###  Devoluciones

El rango.


```python
def get_range(self, recalculate):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| recalculate | bool | si recalcularlo si este nombre ha sido calculado antes de esta invocación.|


##  get_range(sheet_index, row, column) {#int-int-int}
Obtiene el rango si este nombre hace referencia a un rango.
Si la referencia de este nombre no es absoluta, el rango puede ser diferente para diferentes celdas.


###  Devoluciones

El rango.


```python
def get_range(self, sheet_index, row, column):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| sheet_index | int | El índice de hoja correspondiente.|
| row | int | El índice de fila correspondiente.|
| column | int | El índice de columna correspondiente|



###  Ver también
* módulo [aspose.cells](../../)
* clase [Name](/cells/es/python-net/aspose.cells/name)
