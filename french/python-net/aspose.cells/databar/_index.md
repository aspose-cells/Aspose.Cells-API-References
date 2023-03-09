---
title: DataBar classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 400
url: /fr/python-net/aspose.cells/databar/
is_root: false
---
##  DataBar classe
 Décrivez la règle de mise en forme conditionnelle DataBar.
Cette règle de mise en forme conditionnelle affiche une note
barre de données dans la plage de cellules.



Le type DataBar expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [axis_color](/cells/fr/python-net/aspose.cells/databar/axis_color) | Obtient la couleur de l'axe pour les cellules avec une mise en forme conditionnelle sous forme de barres de données.|
| [axis_position](/cells/fr/python-net/aspose.cells/databar/axis_position) | Obtient ou définit la position de l'axe des barres de données spécifiées par une règle de mise en forme conditionnelle.|
| [bar_fill_type](/cells/fr/python-net/aspose.cells/databar/bar_fill_type) | Obtient ou définit la façon dont une barre de données est remplie de couleur.|
| [direction](/cells/fr/python-net/aspose.cells/databar/direction) |Obtient ou définit la direction d'affichage de la barre de données.|
| [bar_border](/cells/fr/python-net/aspose.cells/databar/bar_border) | Obtient un objet qui spécifie la bordure d'une barre de données.|
| [negative_bar_format](/cells/fr/python-net/aspose.cells/databar/negative_bar_format) | Obtient l'objet NegativeBarFormat associé à une règle de mise en forme conditionnelle de la barre de données.|
| [min_cfvo](/cells/fr/python-net/aspose.cells/databar/min_cfvo) | Obtenez ou définissez l'objet de valeur min de cette DataBar.<br/> Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Max.|
| [max_cfvo](/cells/fr/python-net/aspose.cells/databar/max_cfvo) | Obtenir ou définir l'objet de valeur maximale de cette DataBar.<br/> Impossible de définir null ou CFValueObject avec le type FormatConditionValueType.Min.|
| [color](/cells/fr/python-net/aspose.cells/databar/color) | Obtenir ou définir la couleur de cette DataBar.|
| [min_length](/cells/fr/python-net/aspose.cells/databar/min_length) | Représente la longueur minimale de la barre de données.|
| [max_length](/cells/fr/python-net/aspose.cells/databar/max_length) | Représente la longueur maximale de la barre de données .|
| [show_value](/cells/fr/python-net/aspose.cells/databar/show_value) | Obtenir ou définir le drapeau indiquant s'il faut afficher les valeurs des cellules sur lesquelles cette barre de données est appliquée.<br/> La valeur par défaut est true.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [to_image(cell, img_opts)](/cells/fr/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) | Rendre la barre de données dans la cellule en tableau d'octets d'image.|



###  Exemples

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

###  Voir également
* module [aspose.cells](..)
