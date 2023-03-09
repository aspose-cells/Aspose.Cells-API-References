---
title: start_row método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells/lightcellsdataprovider/start_row/
is_root: false
---
##  start_row(row) {#Row}
Comienza a guardar datos de una fila.



```python
def start_row(self, row):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| row | [Row](/cells/es/python-net/aspose.cells/row) | Objeto de fila para la implementación para completar datos. Su índice de fila es el valor devuelto de la última llamada de [LightCellsDataProvider.next_row()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/next_row).<br/>Si la fila se ha inicializado en el modelo de celdas internas, se utilizará el objeto de fila existente.<br/> De lo contrario, se utilizará un objeto Fila temporal para la implementación para completar los datos.|
###  Observaciones

Se llamará al comienzo de guardar una fila y los datos de sus celdas.
Si la fila actual tiene algunas propiedades personalizadas, como altura, estilo, etc.,
la implementación debe establecer esas propiedades en el objeto Row dado aquí.


###  Ver también
* módulo [aspose.cells](../../)
* clase [LightCellsDataProvider](/cells/es/python-net/aspose.cells/lightcellsdataprovider)
