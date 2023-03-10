---
title: IconSet Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 900
url: /de/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet Klasse
 Beschreiben Sie die bedingte Formatierungsregel IconSet.
Diese bedingte Formatierungsregel wendet Symbole auf Zellen an
nach ihren Werten.



Der Typ IconSet macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [cf_icons](/cells/de/python-net/aspose.cells/iconset/cf_icons) | Holen Sie sich die [ConditionalFormattingIcon](/cells/de/python-net/aspose.cells/conditionalformattingicon) aus der Kollektion|
| [cfvos](/cells/de/python-net/aspose.cells/iconset/cfvos) | Rufen Sie die CFValueObjects-Instanz ab.|
| [type](/cells/de/python-net/aspose.cells/iconset/type) | Abrufen oder Festlegen des anzuzeigenden Symbolsatztyps.<br/>Durch das Festlegen des Typs wird automatisch überprüft, ob die aktuelle Cfvos-Zählung lautet<br/> dem neuen Typ entsprechen. Wenn nicht übereinstimmen, werden alte Cfvos gereinigt und<br/> Standard-Cfvos werden hinzugefügt.|
| [is_custom](/cells/de/python-net/aspose.cells/iconset/is_custom) | Gibt an, ob der Symbolsatz benutzerdefiniert ist.<br/> Der Standardwert ist falsch.|
| [show_value](/cells/de/python-net/aspose.cells/iconset/show_value) | Holen oder setzen Sie das Flag, das angibt, ob die Werte der Zellen angezeigt werden sollen, auf die dieser Symbolsatz angewendet wird.<br/> Der Standardwert ist wahr.|
| [reverse](/cells/de/python-net/aspose.cells/iconset/reverse) | Holen oder setzen Sie das Flag, das angibt, ob die Standardreihenfolge der Symbole in diesem Symbolsatz umgekehrt werden soll.<br/> Der Standardwert ist falsch.|



###  Beispiel

```python
from aspose.cells import CellArea, FormatConditionType, IconSetType, Workbook

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
idx = fcs.add_condition(FormatConditionType.ICON_SET)
fcs.add_area(ca)
cond = fcs[idx]
# Get Icon Set
iconSet = cond.icon_set
# Set Icon Type
iconSet.type = IconSetType.ARROWS3
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
* Klasse [ConditionalFormattingIcon](/cells/de/python-net/aspose.cells/conditionalformattingicon)
