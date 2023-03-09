---
title: Column klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 260
url: /sv/python-net/aspose.cells/column/
is_root: false
---
##  Column klass
Representerar en enda kolumn i ett kalkylblad.



Typen Column avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [index](/cells/sv/python-net/aspose.cells/column/index) | Hämtar indexet för denna kolumn.|
| [width](/cells/sv/python-net/aspose.cells/column/width) | Hämtar och ställer in kolumnbredden i teckenenhet.|
| [group_level](/cells/sv/python-net/aspose.cells/column/group_level) | Hämtar gruppnivån för kolumnen.|
| [is_hidden](/cells/sv/python-net/aspose.cells/column/is_hidden) | Indikerar om kolumnen är dold.|
| [has_custom_style](/cells/sv/python-net/aspose.cells/column/has_custom_style) | Indikerar om den här kolumnen har anpassade stilinställningar (som skiljer sig från standarden som ärvts från arbetsboken).|
| [style](/cells/sv/python-net/aspose.cells/column/style) | Får stilen i denna kolumn.|
| [is_collapsed](/cells/sv/python-net/aspose.cells/column/is_collapsed) | om kolumnen är kollapsad|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [apply_style(style, flag)](/cells/sv/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Tillämpar format för en hel kolumn.|
| [get_style()](/cells/sv/python-net/aspose.cells/column/get_style/#) | Får stilen i denna kolumn.|
| [set_style(style)](/cells/sv/python-net/aspose.cells/column/set_style/#Style) | Ställer in stilen för denna kolumn.|



###  Exempel

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first Column
column = worksheet.cells.columns[0]
# Apply Style to first Column
column.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells](..)
