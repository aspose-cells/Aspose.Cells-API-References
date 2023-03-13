---
title: Column Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 260
url: /de/python-net/aspose.cells/column/
is_root: false
---
##  Column Klasse
Stellt eine einzelne Spalte in einem Arbeitsblatt dar.



Der Typ Column macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [index](/cells/de/python-net/aspose.cells/column/index) | Ruft den Index dieser Spalte ab.|
| [width](/cells/de/python-net/aspose.cells/column/width) | Ruft die Spaltenbreite in Zeicheneinheiten ab und legt sie fest.|
| [group_level](/cells/de/python-net/aspose.cells/column/group_level) |Ruft die Gruppenebene der Spalte ab.|
| [is_hidden](/cells/de/python-net/aspose.cells/column/is_hidden) | Gibt an, ob die Spalte ausgeblendet ist.|
| [has_custom_style](/cells/de/python-net/aspose.cells/column/has_custom_style) | Gibt an, ob diese Spalte über benutzerdefinierte Stileinstellungen verfügt (anders als die von der Arbeitsmappe geerbte Standardeinstellung).|
| [style](/cells/de/python-net/aspose.cells/column/style) | Ruft den Stil dieser Spalte ab.|
| [is_collapsed](/cells/de/python-net/aspose.cells/column/is_collapsed) | ob die Spalte zugeklappt ist|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [apply_style(style, flag)](/cells/de/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Wendet Formate für eine ganze Spalte an.|
| [get_style()](/cells/de/python-net/aspose.cells/column/get_style/#) | Ruft den Stil dieser Spalte ab.|
| [set_style(style)](/cells/de/python-net/aspose.cells/column/set_style/#Style) | Legt den Stil dieser Spalte fest.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells](..)
