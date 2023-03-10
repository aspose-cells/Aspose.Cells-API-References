---
title: classe FontSetting
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 670
url: /it/python-net/aspose.cells/fontsetting/
is_root: false
---
##  classe FontSetting
Rappresenta un intervallo di caratteri all'interno del testo della cella.



Il tipo FontSetting espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [FontSetting(start_index, length, sheets)](/cells/it/python-net/aspose.cells/fontsetting/__init__/#int-int-WorksheetCollection) |  |


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [type](/cells/it/python-net/aspose.cells/fontsetting/type) | Ottiene il tipo di nodo di testo.|
| [start_index](/cells/it/python-net/aspose.cells/fontsetting/start_index) | Ottiene l'indice iniziale dei caratteri.|
| [length](/cells/it/python-net/aspose.cells/fontsetting/length) |Ottiene la lunghezza dei caratteri.|
| [font](/cells/it/python-net/aspose.cells/fontsetting/font) | Restituisce il carattere di questo oggetto.|
| [text_options](/cells/it/python-net/aspose.cells/fontsetting/text_options) | Restituisce le opzioni di testo.|


###  Metodi
| Metodo| Descrizione|
| :- | :- |
| [set_word_art_style(style)](/cells/it/python-net/aspose.cells/fontsetting/set_word_art_style/#aspose.cells.drawing.PresetWordArtStyle) | Imposta lo stile WordArt predefinito.|



###  Esempio

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

###  Guarda anche
* modulo [aspose.cells](..)
