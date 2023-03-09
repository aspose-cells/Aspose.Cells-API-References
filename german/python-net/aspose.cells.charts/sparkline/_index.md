---
title: Sparkline Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 260
url: /de/python-net/aspose.cells.charts/sparkline/
is_root: false
---
##  Sparkline Klasse
Eine Sparkline stellt ein winziges Diagramm oder eine Grafik in einer Arbeitsblattzelle dar, die eine visuelle Darstellung von Daten bietet.



Der Typ Sparkline macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [data_range](/cells/de/python-net/aspose.cells.charts/sparkline/data_range) | Repräsentiert den Datenbereich der Sparkline.|
| [row](/cells/de/python-net/aspose.cells.charts/sparkline/row) | Ruft den Zeilenindex der Sparkline ab.|
| [column](/cells/de/python-net/aspose.cells.charts/sparkline/column) | Ruft den Spaltenindex der Sparkline ab.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [to_image(file_name, options)](/cells/de/python-net/aspose.cells.charts/sparkline/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) | Konvertiert eine Sparkline in ein Bild.|
| [to_image(stream, options)](/cells/de/python-net/aspose.cells.charts/sparkline/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) | Konvertiert eine Sparkline in ein Bild.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells.charts](..)
