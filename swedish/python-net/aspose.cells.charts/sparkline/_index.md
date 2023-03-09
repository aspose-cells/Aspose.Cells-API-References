---
title: Sparkline klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 260
url: /sv/python-net/aspose.cells.charts/sparkline/
is_root: false
---
##  Sparkline klass
En sparkline representerar ett litet diagram eller grafik i en kalkylbladscell som ger en visuell representation av data.



Typen Sparkline avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [data_range](/cells/sv/python-net/aspose.cells.charts/sparkline/data_range) | Representerar dataintervallet för sparkline.|
| [row](/cells/sv/python-net/aspose.cells.charts/sparkline/row) | Hämtar radindex för sparkline.|
| [column](/cells/sv/python-net/aspose.cells.charts/sparkline/column) | Hämtar kolumnindex för sparkline.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [to_image(file_name, options)](/cells/sv/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Konverterar en sparkline till en bild.|
| [to_image(stream, options)](/cells/sv/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Konverterar en sparkline till en bild.|



###  Exempel

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

###  Se även
* modul [aspose.cells.charts](..)
