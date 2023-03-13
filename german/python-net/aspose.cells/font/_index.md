---
title: Font Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 650
url: /de/python-net/aspose.cells/font/
is_root: false
---
##  Font Klasse
Kapselt das in einer Tabelle verwendete Schriftobjekt.



Der Typ Font macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [charset](/cells/de/python-net/aspose.cells/font/charset) | Stellt den Zeichensatz dar.|
| [is_italic](/cells/de/python-net/aspose.cells/font/is_italic) | Ruft einen Wert ab, der angibt, ob die Schriftart kursiv ist, oder legt diesen fest.|
| [is_bold](/cells/de/python-net/aspose.cells/font/is_bold) |Ruft einen Wert ab, der angibt, ob die Schriftart fett ist, oder legt diesen fest.|
| [caps_type](/cells/de/python-net/aspose.cells/font/caps_type) | Ruft den Textbegrenzungstyp ab und legt ihn fest.|
| [strike_type](/cells/de/python-net/aspose.cells/font/strike_type) | Ruft den Strike-Typ des Textes ab.|
| [is_strikeout](/cells/de/python-net/aspose.cells/font/is_strikeout) | Ruft einen Wert ab, der angibt, ob die Schriftart einfach durchgestrichen ist, oder legt diesen fest.|
| [script_offset](/cells/de/python-net/aspose.cells/font/script_offset) | Ruft den Skript-Offset in Prozent ab und legt ihn fest|
| [is_superscript](/cells/de/python-net/aspose.cells/font/is_superscript) | Ruft einen Wert ab, der angibt, ob es sich bei der Schriftart um Superskript handelt, oder legt diesen fest.|
| [is_subscript](/cells/de/python-net/aspose.cells/font/is_subscript) | Ruft einen Wert ab, der angibt, ob die Schriftart tiefgestellt ist, oder legt diesen fest.|
| [underline](/cells/de/python-net/aspose.cells/font/underline) | Ruft den Unterstreichungstyp der Schriftart ab oder legt diesen fest.|
| [name](/cells/de/python-net/aspose.cells/font/name) | Ruft den Namen von [Font](/cells/de/python-net/aspose.cells/font) ab oder legt diesen fest.|
| [double_size](/cells/de/python-net/aspose.cells/font/double_size) | Ruft die doppelte Größe der Schriftart ab und legt sie fest.|
| [size](/cells/de/python-net/aspose.cells/font/size) | Ruft die Größe der Schriftart ab oder legt diese fest.|
| [theme_color](/cells/de/python-net/aspose.cells/font/theme_color) | Ruft die Designfarbe ab und legt sie fest.|
| [color](/cells/de/python-net/aspose.cells/font/color) | Ruft die Farbe der Schriftart ab oder legt sie fest.|
| [argb_color](/cells/de/python-net/aspose.cells/font/argb_color) | Ruft die Farbe mit einem 32-Bit-ARGB-Wert ab und legt sie fest.|
| [is_normalize_heights](/cells/de/python-net/aspose.cells/font/is_normalize_heights) | Gibt an, ob die Normalisierung der Höhe auf den Textverlauf angewendet werden soll.|
| [scheme_type](/cells/de/python-net/aspose.cells/font/scheme_type) | Ruft den Schematyp der Schriftart ab und legt ihn fest.|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [equals(font)](/cells/de/python-net/aspose.cells/font/equals/#Font) | Überprüft, ob zwei Schriftarten gleich sind.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)
* Klasse [Font](/cells/de/python-net/aspose.cells/font)
