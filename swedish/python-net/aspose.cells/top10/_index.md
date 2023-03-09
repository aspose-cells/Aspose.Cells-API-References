---
title: Top10 klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1480
url: /sv/python-net/aspose.cells/top10/
is_root: false
---
##  Top10 klass
 Beskriv Top10 villkorlig formateringsregel.
Denna regel för villkorlig formatering markerar celler vars
värden hamnar i den övre N- eller nedre N-parentesen, som specificerats.



Typen Top10 avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [Top10()](/cells/sv/python-net/aspose.cells/top10/__init__/#) | Konstruerar en ny instans av Top10|


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_percent](/cells/sv/python-net/aspose.cells/top10/is_percent) | Hämta eller ställ in om en "topp/botten n"-regel är en "topp/botten n procent"-regel.<br/> Standardvärdet är falskt.|
| [is_bottom](/cells/sv/python-net/aspose.cells/top10/is_bottom) | Hämta eller ställ in om en "top/bottom n"-regel är en "bottom n"-regel.<br/> Standardvärdet är falskt.|
| [rank](/cells/sv/python-net/aspose.cells/top10/rank) | Hämta eller ställ in värdet på "n" i en "top/bottom n" villkorlig formateringsregel.<br/>Om IsPercent är sant måste värdet mellan 0 och 100.<br/>Annars måste den vara mellan 0 och 1000.<br/> Standardvärdet är 10.|



###  Exempel

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

###  Se även
* modul [aspose.cells](..)
