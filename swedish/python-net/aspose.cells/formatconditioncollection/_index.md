---
title: FormatConditionCollection klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 700
url: /sv/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
##  FormatConditionCollection klass
Representerar villkorlig formatering.
Formatvillkoren kan innehålla upp till tre villkorliga format.



Typen FormatConditionCollection avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [count](/cells/sv/python-net/aspose.cells/formatconditioncollection/count) | Får räkningen av villkoren.|
| [range_count](/cells/sv/python-net/aspose.cells/formatconditioncollection/range_count) | Hämtar antalet villkorligt formaterade intervall.|



Hämtar formateringsvillkoret efter index.
###  Indexerare
| namn| Beskrivning|
| :- | :- |
| [index] | indexet för formateringsvillkoret som ska returneras.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/sv/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | Lägger till ett formateringsvillkor.|
| [add_condition(type)](/cells/sv/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) |Lägg till ett formatvillkor.|
| [remove_area(index)](/cells/sv/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Tar bort villkorligt formaterat cellintervall efter index.|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/sv/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Ta bort villkorlig formatering i intervallet.|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/sv/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | Lägger till ett formateringsvillkor och påverkad cellring till FormatConditions<br/>Formatvillkoren kan innehålla upp till tre villkorliga format.<br/> Referenser till de andra arken är inte tillåtna i formlerna för villkorlig formatering.|
| [add_area(cell_area)](/cells/sv/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | Lägger till ett villkorligt formaterat cellintervall.|
| [get_cell_area(index)](/cells/sv/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Hämtar det villkorligt formaterade cellintervallet efter index.|
| [remove_condition(index)](/cells/sv/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Tar bort formateringsvillkoret genom index.|



###  Exempel

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

###  Se även
* modul [aspose.cells](..)
