---
title: Row Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1300
url: /de/python-net/aspose.cells/row/
is_root: false
---
##  Row Klasse
Stellt eine einzelne Zeile in einem Arbeitsblatt dar.



Der Typ Row macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [is_blank](/cells/de/python-net/aspose.cells/row/is_blank) | Gibt an, ob die Zeile Daten enthält|
| [is_collapsed](/cells/de/python-net/aspose.cells/row/is_collapsed) | ob die Zeile reduziert ist|
| [height](/cells/de/python-net/aspose.cells/row/height) | Ruft die Zeilenhöhe in Punkteinheiten ab und legt sie fest.|
| [is_hidden](/cells/de/python-net/aspose.cells/row/is_hidden) | Gibt an, ob die Zeile ausgeblendet ist.|
| [index](/cells/de/python-net/aspose.cells/row/index) | Ruft den Index dieser Zeile ab.|
| [group_level](/cells/de/python-net/aspose.cells/row/group_level) | Ruft die Gruppenebene der Zeile ab.|
| [is_height_matched](/cells/de/python-net/aspose.cells/row/is_height_matched) |Gibt an, dass die Zeilenhöhe und die Standardschrifthöhe übereinstimmen.|
| [style](/cells/de/python-net/aspose.cells/row/style) | Stellt den Stil dieser Zeile dar.|
| [has_custom_style](/cells/de/python-net/aspose.cells/row/has_custom_style) | Gibt an, ob diese Zeile über benutzerdefinierte Stileinstellungen verfügt (anders als die von der Arbeitsmappe geerbte Standardeinstellung).|
| [first_cell](/cells/de/python-net/aspose.cells/row/first_cell) | Ruft das erste Zellobjekt in der Zeile ab.|
| [first_data_cell](/cells/de/python-net/aspose.cells/row/first_data_cell) | Ruft die erste nicht leere Zelle in der Zeile ab.|
| [last_cell](/cells/de/python-net/aspose.cells/row/last_cell) | Ruft das letzte Zellobjekt in der Zeile ab.|
| [last_data_cell](/cells/de/python-net/aspose.cells/row/last_data_cell) | Ruft die letzte nicht leere Zelle in der Zeile ab.|



Ruft die Zelle ab.
###  Indexierer
| Name| Beschreibung|
| :- | :- |
| [index] | Der Spaltenindex|


###  Methoden
| Methode| Beschreibung|
| :- | :- |
| [get_cell_by_index(index)](/cells/de/python-net/aspose.cells/row/get_cell_by_index/#int) | Rufen Sie die Zelle nach einem bestimmten Index in der Liste ab.|
| [get_cell_or_null(column)](/cells/de/python-net/aspose.cells/row/get_cell_or_null/#int) | Ruft die Zelle oder Null im spezifischen Index ab.|
| [get_style()](/cells/de/python-net/aspose.cells/row/get_style/#) | Ruft den Stil dieser Zeile ab.|
| [set_style(style)](/cells/de/python-net/aspose.cells/row/set_style/#Style) | Legt den Stil dieser Zeile fest.|
| [copy_settings(source, check_style)](/cells/de/python-net/aspose.cells/row/copy_settings/#Row-bool) | Kopieren Sie die Einstellungen der Zeile, wie z. B. Stil, Höhe, Sichtbarkeit usw.|
| [apply_style(style, flag)](/cells/de/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Wendet Formate für eine ganze Zeile an.|
| [equals(row)](/cells/de/python-net/aspose.cells/row/equals/#Row) | Überprüft, ob dieses Objekt mit einem anderen Zeilenobjekt auf dieselbe Zeile verweist.|



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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Siehe auch
* Modul [aspose.cells](..)
