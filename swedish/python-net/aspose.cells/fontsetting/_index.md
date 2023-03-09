---
title: FontSetting klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 670
url: /sv/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting klass
Representerar ett teckenintervall i celltexten.



Typen FontSetting avslöjar följande medlemmar:

###  Konstruktörer
| Konstruktör| Beskrivning|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/sv/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [type](/cells/sv/python-net/aspose.cells/fontsetting/type) | Hämtar typen av textnod.|
| [start_index](/cells/sv/python-net/aspose.cells/fontsetting/start_index) | Hämtar startindex för tecknen.|
| [length](/cells/sv/python-net/aspose.cells/fontsetting/length) |Får längden på karaktärerna.|
| [font](/cells/sv/python-net/aspose.cells/fontsetting/font) | Returnerar teckensnittet för detta objekt.|
| [text_options](/cells/sv/python-net/aspose.cells/fontsetting/text_options) | Returnerar textalternativen.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [set_word_art_style(style)](/cells/sv/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Ställer in den förinställda WordArt-stilen.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Visit Aspose!")
# getting charactor
charactor = cell.characters(6, 7)
# Setting the font of selected characters to bold
charactor.font.is_bold = True
# Setting the font color of selected characters to blue
charactor.font.color = Color.blue
# Saving the Excel file
workbook.save("book1.xls")

```

###  Se även
* modul [aspose.cells](..)
