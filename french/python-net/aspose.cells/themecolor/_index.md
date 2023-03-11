---
title: ThemeColor classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1430
url: /fr/python-net/aspose.cells/themecolor/
is_root: false
---
##  ThemeColor classe
Représente une couleur de thème.



Le type ThemeColor expose les membres suivants :

###  Constructeurs
| Constructeur| Description|
| :- | :- |
| [ThemeColor(type, tint)](/cells/fr/python-net/aspose.cells/themecolor/__init__/#ThemeColorType-float) |  |


###  Propriétés
| Propriété| Description|
| :- | :- |
| [color_type](/cells/fr/python-net/aspose.cells/themecolor/color_type) | Obtient et définit le type de thème.|
| [tint](/cells/fr/python-net/aspose.cells/themecolor/tint) | Obtient et définit la valeur de teinte.|



###  Exemple

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

###  Voir également
* module [aspose.cells](..)
