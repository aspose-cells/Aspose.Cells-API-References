---
title: IconSet klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 900
url: /sv/python-net/aspose.cells/iconset/
is_root: false
---
##  IconSet klass
 Beskriv IconSet villkorlig formateringsregel.
Denna regel för villkorlig formatering tillämpar ikoner på celler
enligt deras värderingar.



Typen IconSet avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [cf_icons](/cells/sv/python-net/aspose.cells/iconset/cf_icons) | Få [ConditionalFormattingIcon](/cells/sv/python-net/aspose.cells/conditionalformattingicon) från samlingen|
| [cfvos](/cells/sv/python-net/aspose.cells/iconset/cfvos) | Hämta CFValueObjects-instansen.|
| [type](/cells/sv/python-net/aspose.cells/iconset/type) | Hämta eller Ställ in vilken typ av ikonuppsättning som ska visas.<br/>Att ställa in typen kommer att automatiskt kontrollera om det aktuella Cfvos antal är<br/> överensstämmer med den nya typen. Om inte, kommer gamla Cfvos att rengöras och<br/> standard Cfvos kommer att läggas till.|
| [is_custom](/cells/sv/python-net/aspose.cells/iconset/is_custom) | Indikerar om ikonuppsättningen är anpassad.<br/> Standardvärdet är falskt.|
| [show_value](/cells/sv/python-net/aspose.cells/iconset/show_value) | Hämta eller ställ in flaggan som anger om värdena för cellerna som denna ikonuppsättning tillämpas på ska visas.<br/> Standardvärdet är sant.|
| [reverse](/cells/sv/python-net/aspose.cells/iconset/reverse) | Hämta eller ställ in flaggan som anger om standardordningen för ikonerna i denna ikonuppsättning ska ändras.<br/> Standardvärdet är falskt.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
* klass [ConditionalFormattingIcon](/cells/sv/python-net/aspose.cells/conditionalformattingicon)
