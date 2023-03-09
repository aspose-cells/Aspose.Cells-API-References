---
title: LightCellsDataHandler clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 990
url: /es/python-net/aspose.cells/lightcellsdatahandler/
is_root: false
---
##  LightCellsDataHandler clase
Representa el controlador de datos de celdas para leer archivos de hojas de cálculo grandes en modo ligero.



El tipo LightCellsDataHandler expone los siguientes miembros:

###  Métodos
| Método| Descripción|
| :- | :- |
| [start_sheet(sheet)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_sheet/#Worksheet) | Comienza a procesar una hoja de trabajo.|
| [start_row(row_index)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_row/#int) | Se prepara para procesar una fila.|
| [process_row(row)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_row/#Row) | Comienza a procesar una fila.|
| [start_cell(column_index)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_cell/#int) | Se prepara para procesar una celda.|
| [process_cell(cell)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_cell/#Cell) | Comienza a procesar una celda.|



###  Observaciones

Al leer un libro de trabajo en este modo, se verificará [LightCellsDataHandler.start_sheet(sheet)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_sheet) al leer cada hoja de trabajo en el libro de trabajo.
Para una hoja, si [LightCellsDataHandler.start_sheet(sheet)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_sheet) da verdadero, entonces se verificarán todos los datos y propiedades de las filas/celdas de esta hoja
y procesada por la implementación de esta interfaz. Para cada fila, se llamará al [LightCellsDataHandler.start_row(row_index)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_row) para verificar si es necesario procesarla.
Si es necesario procesar una fila, las propiedades de esta fila se leerán primero y el usuario puede acceder a sus propiedades por [LightCellsDataHandler.process_row(row)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_row).
si las celdas de la fila también deben procesarse, entonces [LightCellsDataHandler.process_row(row)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_row) debería devolver verdadero y luego [LightCellsDataHandler.start_cell(column_index)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/start_cell) será
llamado para cada celda existente en esta fila para verificar si una celda necesita ser procesada.
luego se llamará al [LightCellsDataHandler.process_cell(cell)](/cells/es/python-net/aspose.cells/lightcellsdatahandler/process_cell) para procesar la celda mediante la implementación de esta interfaz.

###  Ver también
* módulo [aspose.cells](..)
