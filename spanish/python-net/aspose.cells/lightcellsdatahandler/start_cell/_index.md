---
title: start_cell método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 40
url: /es/python-net/aspose.cells/lightcellsdatahandler/start_cell/
is_root: false
---
##  start_cell(column_index) {#int}
Se prepara para procesar una celda.


###  Devoluciones

si esta celda necesita ser procesada.false para ignorar la celda y verificar la siguiente hasta llegar al final de los datos de celdas de la fila actual


```python
def start_cell(self, column_index):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| column_index | int | índice de columna de la celda a procesar|
###  Observaciones

Se llamará cuando llegue a una celda existente en la fila actual. La fila actual es la fila de la última llamada de [LightCellsDataHandler.process_row(row)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_row).


###  Ver también

* módulo [aspose.cells](../../)
* clase [LightCellsDataHandler](/cells/es/python-net/aspose.cells/lightcellsdatahandler)
