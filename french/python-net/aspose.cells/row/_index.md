---
title: Row classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1300
url: /fr/python-net/aspose.cells/row/
is_root: false
---
##  Row classe
Représente une seule ligne dans une feuille de calcul.



Le type Row expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_blank](/cells/fr/python-net/aspose.cells/row/is_blank) | Indique si la ligne contient des données|
| [is_collapsed](/cells/fr/python-net/aspose.cells/row/is_collapsed) | si la ligne est réduite|
| [height](/cells/fr/python-net/aspose.cells/row/height) | Obtient et définit la hauteur de la ligne en unités de Points.|
| [is_hidden](/cells/fr/python-net/aspose.cells/row/is_hidden) | Indique si la ligne est masquée.|
| [index](/cells/fr/python-net/aspose.cells/row/index) | Obtient l'index de cette ligne.|
| [group_level](/cells/fr/python-net/aspose.cells/row/group_level) | Obtient le niveau de groupe de la ligne.|
| [is_height_matched](/cells/fr/python-net/aspose.cells/row/is_height_matched) | Indique que la hauteur de ligne et la hauteur de police par défaut correspondent.|
| [style](/cells/fr/python-net/aspose.cells/row/style) | Représente le style de cette ligne.|
| [has_custom_style](/cells/fr/python-net/aspose.cells/row/has_custom_style) | Indique si cette ligne a des paramètres de style personnalisés (différents de ceux par défaut hérités du classeur).|
| [first_cell](/cells/fr/python-net/aspose.cells/row/first_cell) | Obtient le premier objet cellule de la ligne.|
| [first_data_cell](/cells/fr/python-net/aspose.cells/row/first_data_cell) | Obtient la première cellule non vide de la ligne.|
| [last_cell](/cells/fr/python-net/aspose.cells/row/last_cell) |Obtient le dernier objet cellule de la ligne.|
| [last_data_cell](/cells/fr/python-net/aspose.cells/row/last_data_cell) | Obtient la dernière cellule non vide de la ligne.|



Obtient la cellule.
###  Indexeur
| Nom| Description|
| :- | :- |
| [index] | L'indice de colonne|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get_cell_by_index(index)](/cells/fr/python-net/aspose.cells/row/get_cell_by_index/#int) | Obtenez la cellule par index spécifique dans la liste.|
| [get_cell_or_null(column)](/cells/fr/python-net/aspose.cells/row/get_cell_or_null/#int) | Obtient la cellule ou null dans l'index spécifique.|
| [get_style()](/cells/fr/python-net/aspose.cells/row/get_style/#) | Obtient le style de cette ligne.|
| [set_style(style)](/cells/fr/python-net/aspose.cells/row/set_style/#Style) | Définit le style de cette ligne.|
| [copy_settings(source, check_style)](/cells/fr/python-net/aspose.cells/row/copy_settings/#Row-bool) | Copiez les paramètres de la ligne, tels que le style, la hauteur, la visibilité, etc.|
| [apply_style(style, flag)](/cells/fr/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) | Applique les formats pour une ligne entière.|
| [equals(row)](/cells/fr/python-net/aspose.cells/row/equals/#Row) | Vérifie si cet objet fait référence à la même ligne avec un autre objet de ligne.|



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
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

###  Voir également
* module [aspose.cells](..)
