---
title: classe ThemeColor
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 1430
url: /it/python-net/aspose.cells/themecolor/
is_root: false
---
##  classe ThemeColor
Rappresenta un colore del tema.



Il tipo ThemeColor espone i membri seguenti:

###  Costruttori
| Costruttore| Descrizione|
| :- | :- |
| [ThemeColor(type, tint)](/cells/it/python-net/aspose.cells/themecolor/__init__/#ThemeColorType-float) |  |


###  Proprietà
| Proprietà| Descrizione|
| :- | :- |
| [color_type](/cells/it/python-net/aspose.cells/themecolor/color_type) | Ottiene e imposta il tipo di tema.|
| [tint](/cells/it/python-net/aspose.cells/themecolor/tint) | Ottiene e imposta il valore della tinta.|



###  Esempio

```python
from aspose.cells import BackgroundType, ThemeColor, ThemeColorType, Workbook

# Instantiating a Workbook object
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("A1").put_value("Hello World")
style = cells.get("A1").get_style()
# Set ThemeColorType.Text2 color type with 40% lighten as the font color.
style.font.theme_color = ThemeColor(ThemeColorType.TEXT2, 0.4)
style.pattern = BackgroundType.SOLID
# Set ThemeColorType.Background2 color type with 75% darken as the foreground color
style.foreground_theme_color = ThemeColor(ThemeColorType.BACKGROUND2, -0.75)
cells.get("A1").set_style(style)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Guarda anche
* modulo [aspose.cells](..)
