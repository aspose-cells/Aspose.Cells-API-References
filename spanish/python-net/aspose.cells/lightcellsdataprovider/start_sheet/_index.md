---
title: start_sheet método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 70
url: /es/python-net/aspose.cells/lightcellsdataprovider/start_sheet/
is_root: false
---
##  start_sheet(sheet_index) {#int}
Comienza a guardar una hoja de trabajo.


###  Devoluciones

verdadero si este proveedor proporcionará datos para la hoja dada; falso si la hoja dada debe usar su modelo de datos normal (Cells).


```python
def start_sheet(self, sheet_index):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| sheet_index | int | índice de la hoja actual que se va a guardar.|
###  Observaciones

Se llamará al comienzo de guardar una hoja de trabajo durante el guardado de un libro de trabajo.
 Si el proveedor necesita referirse a*`índice de hoja`* más tarde
en el método startRow(Row) o startCell(Cell),
 es decir, si el proceso necesita saber qué hoja de trabajo se está procesando,
 la implementación debe conservar la*`índice de hoja`* valor aquí.


###  Ver también
* módulo [aspose.cells](../../)
* clase [LightCellsDataProvider](/cells/es/python-net/aspose.cells/lightcellsdataprovider)
