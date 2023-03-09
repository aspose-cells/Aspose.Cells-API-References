---
title: LightCellsDataProvider clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 1000
url: /es/python-net/aspose.cells/lightcellsdataprovider/
is_root: false
---
##  LightCellsDataProvider clase
Representa el proveedor de datos para guardar archivos de hojas de cálculo grandes en modo ligero.



El tipo LightCellsDataProvider expone los siguientes miembros:

###  Métodos
| Método| Descripción|
| :- | :- |
| [start_sheet(sheet_index)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_sheet/#int) | Comienza a guardar una hoja de trabajo.|
| [next_row()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/next_row/#) | Obtiene la siguiente fila que se va a guardar.|
| [start_row(row)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_row/#Row) | Comienza a guardar datos de una fila.|
| [next_cell()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/next_cell/#) | Obtiene la siguiente celda que se guardará.|
| [start_cell(cell)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_cell/#Cell) | Comienza a guardar datos de una celda.|
| [is_gather_string()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/is_gather_string/#) |Comprueba si el valor de cadena actual de la celda debe recopilarse en un grupo global.|



###  Observaciones

Al guardar un libro de trabajo con este modo, se verificará [LightCellsDataProvider.start_sheet(sheet_index)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_sheet) al guardar cada hoja de trabajo en el libro de trabajo.
Para una hoja, si [LightCellsDataProvider.start_sheet(sheet_index)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_sheet) da verdadero, entonces se guardarán todos los datos y propiedades de las filas/celdas de esta hoja
será proporcionado por la implementación de esta interfaz.. En primer lugar, se llamará a [LightCellsDataProvider.next_row()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/next_row) para obtener el índice de la siguiente fila que se guardará.
Si se devuelve un índice de fila válido (el índice de fila debe estar en orden ascendente para que se guarden las filas),
luego, se proporcionará un objeto Row que represente esta fila para que la implementación establezca sus propiedades en [LightCellsDataProvider.start_row(row)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_row).
Para una fila, primero se verificará [LightCellsDataProvider.next_cell()](/cells/es/python-net/aspose.cells/lightcellsdataprovider/next_cell). Si se devuelve un índice de columna válido (el índice de columna debe estar en orden ascendente para que se guarden todas las celdas de una fila),
luego, se proporcionará un objeto Cell que representa esta celda para que la implementación establezca sus datos y propiedades en [LightCellsDataProvider.start_cell(cell)](/cells/es/python-net/aspose.cells/lightcellsdataprovider/start_cell).
Después de configurar los datos de esta celda, esta celda se guardará directamente en el archivo de hoja de cálculo generado y la siguiente celda se verificará y procesará.

###  Ver también
* módulo [aspose.cells](..)
