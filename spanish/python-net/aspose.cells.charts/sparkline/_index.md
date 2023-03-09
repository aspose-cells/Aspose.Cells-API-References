---
title: Sparkline clase
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 260
url: /es/python-net/aspose.cells.charts/sparkline/
is_root: false
---
##  Sparkline clase
Un minigráfico representa un cuadro o gráfico diminuto en una celda de una hoja de cálculo que proporciona una representación visual de los datos.



El tipo Sparkline expone los siguientes miembros:

###  Propiedades
| Propiedad| Descripción|
| :- | :- |
| [data_range](/cells/es/python-net/aspose.cells.charts/sparkline/data_range) | Representa el rango de datos del minigráfico.|
| [row](/cells/es/python-net/aspose.cells.charts/sparkline/row) | Obtiene el índice de fila del minigráfico.|
| [column](/cells/es/python-net/aspose.cells.charts/sparkline/column) | Obtiene el índice de columna del minigráfico.|


###  Métodos
| Método| Descripción|
| :- | :- |
| [to_image(file_name, options)](/cells/es/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Convierte un minigráfico en una imagen.|
| [to_image(stream, options)](/cells/es/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Convierte un minigráfico en una imagen.|



###  Ejemplo

```python
from aspose.cells import CellArea, Workbook
from aspose.cells.charts import SparklineType
from aspose.cells.rendering import ImageOrPrintOptions

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, sheet.name + "!A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
idx = group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
line = group.sparkline_collection[idx]
print("Saprkline data range: "  + line.data_range + ", row: "  + str(line.row) + ", column: "  + str(line.column))
line.to_image("output.png", ImageOrPrintOptions())

```

###  Ver también
* módulo [aspose.cells.charts](..)
