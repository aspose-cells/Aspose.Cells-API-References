---
title: process_row método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells/lightcellsdatahandler/process_row/
is_root: false
---
##  process_row(row) {#Row}
Comienza a procesar una fila.


###  Devoluciones

si las celdas de esta fila necesitan ser procesadas. false para ignorar todas las celdas de esta fila.


```python
def process_row(self, row):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| row | [Row](/cells/es/python-net/aspose.cells/row) | Objeto de fila que se está procesando actualmente.|
###  Observaciones

Se llamará después de las propiedades de la fila, como la altura, el estilo, etc. han sido leídos. Sin embargo, las celdas de esta fila aún no se han leído.


###  Ver también

* módulo [aspose.cells](../../)
* clase [LightCellsDataHandler](/cells/es/python-net/aspose.cells/lightcellsdatahandler)
