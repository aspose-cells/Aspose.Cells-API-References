---
title: DataBar Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 400
url: /de/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar Klasse
 Beschreiben Sie die bedingte Formatierungsregel DataBar.
Diese bedingte Formatierungsregel zeigt ein abgestuftes an
Datenleiste im Bereich der Zellen.



Der Typ DataBar macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [axis_color](/cells/de/python-net/aspose.cells/databar/axis_color) | Ruft die Farbe der Achse für Zellen mit bedingter Formatierung als Datenbalken ab.|
| [axis_position](/cells/de/python-net/aspose.cells/databar/axis_position) | Ruft die Position der Achse der Datenbalken ab, die durch eine bedingte Formatierungsregel angegeben ist, oder legt diese fest.|
| [bar_fill_type](/cells/de/python-net/aspose.cells/databar/bar_fill_type) | Ruft ab oder legt fest, wie ein Datenbalken mit Farbe gefüllt wird.|
| [direction](/cells/de/python-net/aspose.cells/databar/direction) |Ruft die Richtung ab, in der die Datenleiste angezeigt wird, oder legt diese fest.|
| [bar_border](/cells/de/python-net/aspose.cells/databar/bar_border) | Ruft ein Objekt ab, das den Rahmen eines Datenbalkens angibt.|
| [negative_bar_format](/cells/de/python-net/aspose.cells/databar/negative_bar_format) | Ruft das NegativeBarFormat-Objekt ab, das einer bedingten Formatierungsregel für Datenbalken zugeordnet ist.|
| [min_cfvo](/cells/de/python-net/aspose.cells/databar/min_cfvo) | Rufen Sie das Mindestwertobjekt dieses DataBar ab oder legen Sie es fest.<br/> Es kann nicht null oder CFValueObject mit dem Typ FormatConditionValueType.Max darauf gesetzt werden.|
| [max_cfvo](/cells/de/python-net/aspose.cells/databar/max_cfvo) | Rufen Sie das Objekt für den maximalen Wert dieses DataBar ab oder legen Sie es fest.<br/> Es kann nicht null oder CFValueObject mit dem Typ FormatConditionValueType.Min darauf gesetzt werden.|
| [color](/cells/de/python-net/aspose.cells/databar/color) | Rufen Sie die Farbe dieses DataBar ab oder legen Sie sie fest.|
| [min_length](/cells/de/python-net/aspose.cells/databar/min_length) | Repräsentiert die Mindestlänge des Datenbalkens .|
| [max_length](/cells/de/python-net/aspose.cells/databar/max_length) | Repräsentiert die maximale Länge des Datenbalkens.|
| [show_value](/cells/de/python-net/aspose.cells/databar/show_value) | Holen oder setzen Sie das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Datenbalken angewendet wird.<br/> Der Standardwert ist wahr.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [to_image(cell, img_opts)](/cells/de/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Rendern Sie den Datenbalken in der Zelle in ein Bild-Byte-Array.|



###  Beispiel

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Siehe auch
* Modul [aspose.cells](..)
