---
title: Top10 Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1480
url: /de/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 Klasse
 Beschreiben Sie die bedingte Formatierungsregel Top10.
Diese Regel zur bedingten Formatierung hebt Zellen hervor, deren
Werte fallen in die obere N- oder untere N-Klammer, wie angegeben.



Der Typ Top10 macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [Top10()](/cells/de/python-net/aspose.cells/top10/__init__/#) |Erstellt eine neue Instanz von Top10|


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_percent](/cells/de/python-net/aspose.cells/top10/is_percent) | Rufen Sie ab oder legen Sie fest, ob eine „Top/Bottom n“-Regel eine „Top/Bottom n Prozent“-Regel ist.<br/> Der Standardwert ist falsch.|
| [is_bottom](/cells/de/python-net/aspose.cells/top10/is_bottom) | Rufen Sie ab oder legen Sie fest, ob eine „Top/Bottom n“-Regel eine „Bottom n“-Regel ist.<br/> Der Standardwert ist falsch.|
| [rank](/cells/de/python-net/aspose.cells/top10/rank) | Abrufen oder Festlegen des Werts von „n“ in einer bedingten Formatierungsregel „top/bottom n“.<br/>Wenn IsPercent wahr ist, muss der Wert zwischen 0 und 100 liegen.<br/>Andernfalls muss er zwischen 0 und 1000 liegen.<br/> Der Standardwert ist 10.|



###  Beispiel

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
