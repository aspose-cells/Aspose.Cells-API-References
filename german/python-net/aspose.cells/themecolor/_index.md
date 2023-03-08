---
title: ThemeColor Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1430
url: /de/python-net/aspose.cells/themecolor/
is_root: false
---
##  ThemeColor Klasse
Stellt eine Designfarbe dar.



Der Typ ThemeColor macht die folgenden Member verfügbar:

###  Konstrukteure
| Konstrukteur| Beschreibung|
| :- | :- |
| [ThemeColor(type, tint)](/cells/de/python-net/aspose.cells/themecolor/__init__/#ThemeColorType-float) |  |


###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [color_type](/cells/de/python-net/aspose.cells/themecolor/color_type) | Ruft den Designtyp ab und legt ihn fest.|
| [tint](/cells/de/python-net/aspose.cells/themecolor/tint) | Ruft den Farbtonwert ab und legt ihn fest.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)
