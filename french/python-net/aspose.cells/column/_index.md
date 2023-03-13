---
title: Column classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 260
url: /fr/python-net/aspose.cells/column/
is_root: false
---
##  Column classe
Représente une seule colonne dans une feuille de calcul.



Le type Column expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [index](/cells/fr/python-net/aspose.cells/column/index) | Obtient l'index de cette colonne.|
| [width](/cells/fr/python-net/aspose.cells/column/width) | Obtient et définit la largeur de la colonne en unité de caractères.|
| [group_level](/cells/fr/python-net/aspose.cells/column/group_level) |Obtient le niveau de groupe de la colonne.|
| [is_hidden](/cells/fr/python-net/aspose.cells/column/is_hidden) | Indique si la colonne est masquée.|
| [has_custom_style](/cells/fr/python-net/aspose.cells/column/has_custom_style) | Indique si cette colonne a des paramètres de style personnalisés (différents de ceux par défaut hérités du classeur).|
| [style](/cells/fr/python-net/aspose.cells/column/style) | Obtient le style de cette colonne.|
| [is_collapsed](/cells/fr/python-net/aspose.cells/column/is_collapsed) | si la colonne est réduite|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [apply_style(style, flag)](/cells/fr/python-net/aspose.cells/column/apply_style/#Style-StyleFlag) | Applique les formats pour une colonne entière.|
| [get_style()](/cells/fr/python-net/aspose.cells/column/get_style/#) | Obtient le style de cette colonne.|
| [set_style(style)](/cells/fr/python-net/aspose.cells/column/set_style/#Style) | Définit le style de cette colonne.|



###  Exemple

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

###  Voir également
* module [aspose.cells](..)
