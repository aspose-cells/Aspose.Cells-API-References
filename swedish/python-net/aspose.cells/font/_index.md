---
title: Font klass
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 650
url: /sv/python-net/aspose.cells/font/
is_root: false
---
##  Font klass
Kapslar in teckensnittsobjektet som används i ett kalkylblad.



Typen Font avslöjar följande medlemmar:

###  Egenskaper
| Fast egendom| Beskrivning|
| :- | :- |
| [charset](/cells/sv/python-net/aspose.cells/font/charset) | Representera teckenuppsättningen.|
| [is_italic](/cells/sv/python-net/aspose.cells/font/is_italic) | Hämtar eller ställer in ett värde som anger om teckensnittet är kursivt.|
| [is_bold](/cells/sv/python-net/aspose.cells/font/is_bold) | Hämtar eller ställer in ett värde som anger om teckensnittet är fetstilt.|
| [caps_type](/cells/sv/python-net/aspose.cells/font/caps_type) | Hämtar och ställer in typ av textkapslar.|
| [strike_type](/cells/sv/python-net/aspose.cells/font/strike_type) | Får textens strejktyp.|
| [is_strikeout](/cells/sv/python-net/aspose.cells/font/is_strikeout) | Hämtar eller ställer in ett värde som indikerar om teckensnittet är enkel genomstruken.|
| [script_offset](/cells/sv/python-net/aspose.cells/font/script_offset) | Hämtar och ställer in skriptoffset, i procentenhet|
| [is_superscript](/cells/sv/python-net/aspose.cells/font/is_superscript) | Hämtar eller ställer in ett värde som anger om teckensnittet är superskript.|
| [is_subscript](/cells/sv/python-net/aspose.cells/font/is_subscript) | Hämtar eller ställer in ett värde som anger om teckensnittet är nedsänkt.|
| [underline](/cells/sv/python-net/aspose.cells/font/underline) | Hämtar eller ställer in teckensnittets understrykningstyp.|
| [name](/cells/sv/python-net/aspose.cells/font/name) | Hämtar eller ställer in namnet på [Font](/cells/sv/python-net/aspose.cells/font).|
| [double_size](/cells/sv/python-net/aspose.cells/font/double_size) | Hämtar och ställer in den dubbla storleken på teckensnittet.|
| [size](/cells/sv/python-net/aspose.cells/font/size) | Hämtar eller ställer in storleken på teckensnittet.|
| [theme_color](/cells/sv/python-net/aspose.cells/font/theme_color) | Får och ställer in temafärgen.|
| [color](/cells/sv/python-net/aspose.cells/font/color) | Hämtar eller ställer in teckensnittets färg.|
| [argb_color](/cells/sv/python-net/aspose.cells/font/argb_color) | Hämtar och ställer in färgen med ett 32-bitars ARGB-värde.|
| [is_normalize_heights](/cells/sv/python-net/aspose.cells/font/is_normalize_heights) | Anger om normaliseringen av höjden som ska tillämpas på texten löper.|
| [scheme_type](/cells/sv/python-net/aspose.cells/font/scheme_type) | Hämtar och ställer in schematypen för teckensnittet.|


###  Metoder
| Metod| Beskrivning|
| :- | :- |
| [equals(font)](/cells/sv/python-net/aspose.cells/font/equals/#Font) | Kontrollerar om två teckensnitt är lika.|



###  Exempel

```python
from aspose.cells import Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Accessing the "A1" cell from the worksheet
cell = worksheet.cells.get("A1")
# Adding some value to the "A1" cell
cell.put_value("Hello Aspose!")
font = cell.get_style().font
# Setting the font name to "Times New Roman"
font.name = "Times New Roman"
# Setting font size to 14
font.size = 14
# setting font color as Red
font.color = Color.red
# Saving the Excel file
workbook.save(r"dest.xls")

```

###  Se även
* modul [aspose.cells](..)
* klass [Font](/cells/sv/python-net/aspose.cells/font)
