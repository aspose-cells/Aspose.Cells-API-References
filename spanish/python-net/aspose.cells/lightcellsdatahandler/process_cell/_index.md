---
title: process_cell método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 20
url: /es/python-net/aspose.cells/lightcellsdatahandler/process_cell/
is_root: false
---
##  process_cell(cell) {#Cell}
Comienza a procesar una celda.


###  Devoluciones

si esta celda debe mantenerse en el modelo de celdas de la hoja actual.
Por lo general, debe ser falso para que todas las celdas no se mantengan en la memoria después de ser procesadas y luego se guarden en la memoria.
Para algún propósito especial, como que el usuario necesite acceder a algunas celdas más tarde después de que se haya procesado todo el libro de trabajo,
el usuario puede hacer que este método se vuelva verdadero para mantener esas celdas especiales en el modelo Cells y acceder a ellas más tarde mediante API como Cells [fila, columna].
Sin embargo, mantener los datos de las celdas en el modelo Cells requerirá más memoria y, si se mantienen todas las celdas, se leerá el archivo de plantilla.
en el modo LightCells será igual al leerlo de forma normal.


```python
def process_cell(self, cell):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| cell | [Cell](/cells/es/python-net/aspose.cells/cell) | Cell objeto que se está procesando actualmente|
###  Observaciones

Se llamará después de que se hayan leído los datos de una celda.


###  Ver también

* módulo [aspose.cells](../../)
* clase [LightCellsDataHandler](/cells/es/python-net/aspose.cells/lightcellsdatahandler)
