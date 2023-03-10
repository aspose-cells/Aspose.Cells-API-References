---
title: get_formula1 método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/formatcondition/get_formula1/
is_root: false
---
##  get_formula1(is_r1c1, is_local) {#bool-bool}
Obtiene el valor o la expresión asociada a esta condición de formato.


###  Devoluciones

El valor o la expresión asociada con esta condición de formato.


```python
def get_formula1(self, is_r1c1, is_local):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| is_r1c1 | bool | Si la fórmula debe formatearse como R1C1.|
| is_local | bool | Si la fórmula debe formatearse según la configuración regional.|


##  get_formula1(row, column) {#int-int}
Obtiene la fórmula del formato condicional de la celda.


###  Devoluciones

La formula.


```python
def get_formula1(self, row, column):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| row | int | El índice de fila.|
| column | int | El índice de la columna.|


##  get_formula1(is_r1c1, is_local, row, column) {#bool-bool-int-int}
Obtiene el valor o la expresión del formato condicional de la celda.


###  Devoluciones

El valor o la expresión asociada con el formato condicional de la celda.


```python
def get_formula1(self, is_r1c1, is_local, row, column):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| is_r1c1 | bool | Si la fórmula debe formatearse como R1C1.|
| is_local | bool | Si la fórmula debe formatearse según la configuración regional.|
| row | int | El índice de fila.|
| column | int | El índice de la columna.|
###  Observaciones

La celda dada debe estar contenida en este formato condicional; de lo contrario, se devolverá un valor nulo.


###  Ver también

* módulo [aspose.cells](../../)
* clase [FormatCondition](/cells/es/python-net/aspose.cells/formatcondition)
