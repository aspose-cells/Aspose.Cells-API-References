---
title: Row klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 1300
url: /sv/python-net/aspose.cells/row/
is_root: false
---
##  Row klass
Representerar en enda rad i ett kalkylblad.



Typen Row avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [is_blank](/cells/sv/python-net/aspose.cells/row/is_blank) | Anger om raden innehåller data|
| [is_collapsed](/cells/sv/python-net/aspose.cells/row/is_collapsed) | om raden är kollapsad|
| [height](/cells/sv/python-net/aspose.cells/row/height) | Hämtar och ställer in radhöjden i enheter av poäng.|
| [is_hidden](/cells/sv/python-net/aspose.cells/row/is_hidden) | Indikerar om raden är dold.|
| [index](/cells/sv/python-net/aspose.cells/row/index) | Hämtar indexet för den här raden.|
| [group_level](/cells/sv/python-net/aspose.cells/row/group_level) | Hämtar radens gruppnivå.|
| [is_height_matched](/cells/sv/python-net/aspose.cells/row/is_height_matched) |Indikerar att radhöjd och standardfonthöjd matchar.|
| [style](/cells/sv/python-net/aspose.cells/row/style) | Representerar stilen på den här raden.|
| [has_custom_style](/cells/sv/python-net/aspose.cells/row/has_custom_style) | Indikerar om den här raden har anpassade stilinställningar (som skiljer sig från standarden som ärvts från arbetsboken).|
| [first_cell](/cells/sv/python-net/aspose.cells/row/first_cell) | Hämtar det första cellobjektet i raden.|
| [first_data_cell](/cells/sv/python-net/aspose.cells/row/first_data_cell) | Får den första icke-tomma cellen i raden.|
| [last_cell](/cells/sv/python-net/aspose.cells/row/last_cell) | Hämtar det sista cellobjektet i raden.|
| [last_data_cell](/cells/sv/python-net/aspose.cells/row/last_data_cell) | Hämtar den sista icke-tomma cellen i raden.|



Får cellen.
###  Indexerare
| namn| Beskrivning|
| :- | :- |
| [index] | Kolumnindex|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [get_cell_by_index(index)](/cells/sv/python-net/aspose.cells/row/get_cell_by_index/#int) | Hämta cellen efter specifikt index i listan.|
| [get_cell_or_null(column)](/cells/sv/python-net/aspose.cells/row/get_cell_or_null/#int) | Hämtar cellen eller null i det specifika indexet.|
| [get_style()](/cells/sv/python-net/aspose.cells/row/get_style/#) | Får stilen på den här raden.|
| [set_style(style)](/cells/sv/python-net/aspose.cells/row/set_style/#Style) | Ställer in stilen för den här raden.|
| [copy_settings(source, check_style)](/cells/sv/python-net/aspose.cells/row/copy_settings/#Row-bool) | Kopiera inställningar för rad, som stil, höjd, synlighet, ... etc.|
| [apply_style(style, flag)](/cells/sv/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Använder format för en hel rad.|
| [equals(row)](/cells/sv/python-net/aspose.cells/row/equals/#Row) | Kontrollerar om detta objekt refererar till samma rad med ett annat radobjekt.|



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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells](..)
