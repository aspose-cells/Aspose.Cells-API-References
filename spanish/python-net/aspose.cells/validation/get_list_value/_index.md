---
title: get_list_value método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/validation/get_list_value/
is_root: false
---
##  get_list_value(row, column) {#int-int}
Obtenga el valor para la lista de la validación de la celda especificada.


###  Devoluciones

El valor para producir la lista de esta validación para la celda especificada.
Si la lista hace referencia a un rango, el valor devuelto será un objeto [ReferredArea](/cells/es/python-net/aspose.cells/referredarea);
De lo contrario, el valor devuelto puede ser nulo, objeto [] u objeto simple.


```python
def get_list_value(self, row, column):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| row | int | El índice de fila.|
| column | int | El índice de la columna.|
###  Observaciones

Solo para validación cuyo tipo es Lista y se ha aplicado a una celda dada,
de lo contrario, se devolverá nulo.


###  Ver también
* módulo [aspose.cells](../../)
* clase [ReferredArea](/cells/es/python-net/aspose.cells/referredarea)
* clase [Validation](/cells/es/python-net/aspose.cells/validation)
