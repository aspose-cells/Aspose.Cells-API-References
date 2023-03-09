---
title: FontSetting Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 670
url: /de/python-net/aspose.cells/fontsetting/
is_root: false
---
##  FontSetting Klasse
Stellt einen Bereich von Zeichen im Zellentext dar.



Der Typ FontSetting macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/de/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [type](/cells/de/python-net/aspose.cells/fontsetting/type) | Ruft den Typ des Textknotens ab.|
| [start_index](/cells/de/python-net/aspose.cells/fontsetting/start_index) | Ruft den Startindex der Zeichen ab.|
| [length](/cells/de/python-net/aspose.cells/fontsetting/length) |Ruft die Länge der Zeichen ab.|
| [font](/cells/de/python-net/aspose.cells/fontsetting/font) | Gibt die Schriftart dieses Objekts zurück.|
| [text_options](/cells/de/python-net/aspose.cells/fontsetting/text_options) | Gibt die Textoptionen zurück.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [set_word_art_style(style)](/cells/de/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Legt den voreingestellten WordArt-Stil fest.|



###  Beispiele

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

###  Siehe auch
* Modul [aspose.cells](..)
