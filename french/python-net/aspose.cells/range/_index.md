---
title: Range classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1250
url: /fr/python-net/aspose.cells/range/
is_root: false
---
##  Range classe
Encapsule l'objet qui représente une plage de cellules dans une feuille de calcul.



Le type Range expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [current_region](/cells/fr/python-net/aspose.cells/range/current_region) |Renvoie un objet Range qui représente la région actuelle.<br/> La région actuelle est une plage délimitée par n'importe quelle combinaison de lignes vides et de colonnes vides.|
| [hyperlinks](/cells/fr/python-net/aspose.cells/range/hyperlinks) | Obtient tous les liens hypertexte de la plage.|
| [row_count](/cells/fr/python-net/aspose.cells/range/row_count) | Obtient le nombre de lignes dans la plage.|
| [column_count](/cells/fr/python-net/aspose.cells/range/column_count) | Obtient le nombre de colonnes dans la plage.|
| [cell_count](/cells/fr/python-net/aspose.cells/range/cell_count) | Obtient tout le nombre de cellules dans la plage.|
| [name](/cells/fr/python-net/aspose.cells/range/name) | Obtient ou définit le nom de la plage.|
| [refers_to](/cells/fr/python-net/aspose.cells/range/refers_to) | Obtient les références de la plage.|
| [address](/cells/fr/python-net/aspose.cells/range/address) | Obtient l'adresse de la plage.|
| [left](/cells/fr/python-net/aspose.cells/range/left) | Obtient la distance, en points, entre le bord gauche de la colonne A et le bord gauche de la plage.|
| [top](/cells/fr/python-net/aspose.cells/range/top) | Obtient la distance, en points, entre le bord supérieur de la ligne 1 et le bord supérieur de la plage.|
| [width](/cells/fr/python-net/aspose.cells/range/width) | Obtient la largeur d'une plage en points.|
| [height](/cells/fr/python-net/aspose.cells/range/height) | Obtient la largeur d'une plage en points.|
| [first_row](/cells/fr/python-net/aspose.cells/range/first_row) | Obtient l'index de la première ligne de la plage.|
| [first_column](/cells/fr/python-net/aspose.cells/range/first_column) | Obtient l'index de la première colonne de la plage.|
| [value](/cells/fr/python-net/aspose.cells/range/value) | Obtient et définit la valeur de la plage.|
| [column_width](/cells/fr/python-net/aspose.cells/range/column_width) | Définit ou obtient la largeur de colonne de cette plage|
| [row_height](/cells/fr/python-net/aspose.cells/range/row_height) | Définit ou obtient la hauteur des lignes dans cette plage|
| [entire_column](/cells/fr/python-net/aspose.cells/range/entire_column) |Obtient un objet Range qui représente la ou les colonnes entières contenant la plage spécifiée.|
| [entire_row](/cells/fr/python-net/aspose.cells/range/entire_row) | Obtient un objet Range qui représente la ligne entière (ou les lignes) contenant la plage spécifiée.|
| [worksheet](/cells/fr/python-net/aspose.cells/range/worksheet) | Obtient l'objet [Range.worksheet](/cells/fr/python-net/aspose.cells/range#worksheet) qui contient cette plage.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [auto_fill(target)](/cells/fr/python-net/aspose.cells/range/auto_fill/#Range) | Remplit automatiquement la plage cible.|
| [auto_fill(target, auto_fill_type)](/cells/fr/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) | Remplit automatiquement la plage cible.|
| [set_style(style, explicit_flag)](/cells/fr/python-net/aspose.cells/range/set_style/#Style-bool) | Appliquez le style de cellule.|
| [set_style(style)](/cells/fr/python-net/aspose.cells/range/set_style/#Style) | Définit le style de la plage.|
| [set_outline_borders(border_style, border_color)](/cells/fr/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) | Définit les bordures de contour autour d'une plage de cellules avec le même style et la même couleur de bordure.|
| [set_outline_borders(border_style, border_color)](/cells/fr/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) | Définit les bordures de contour autour d'une plage de cellules avec le même style et la même couleur de bordure.|
| [set_outline_borders(border_styles, border_colors)](/cells/fr/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) | Définit des bordures de ligne autour d'une plage de cellules.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/fr/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) | Définit une bordure de contour autour d'une plage de cellules.|
| [set_outline_border(border_edge, border_style, border_color)](/cells/fr/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) | Définit une bordure de contour autour d'une plage de cellules.|
| [copy(range, options)](/cells/fr/python-net/aspose.cells/range/copy/#Range-PasteOptions) | Copie de la plage avec des options spéciales de collage.|
| [copy(range)](/cells/fr/python-net/aspose.cells/range/copy/#Range) | Copie les données (y compris les formules), la mise en forme, les objets de dessin, etc. à partir d'une plage source.|
| [get_enumerator()](/cells/fr/python-net/aspose.cells/range/get_enumerator/#) | Obtient l'énumérateur des cellules de cette plage.|
| [is_intersect(range)](/cells/fr/python-net/aspose.cells/range/is_intersect/#Range) | Indique si la plage est intersectée.|
| [intersect(range)](/cells/fr/python-net/aspose.cells/range/intersect/#Range) | Renvoie un objet [Range](/cells/fr/python-net/aspose.cells/range) qui représente l'intersection rectangulaire de deux plages.|
| [union(range)](/cells/fr/python-net/aspose.cells/range/union/#Range) | Renvoie l'union de deux plages.|
| [merge()](/cells/fr/python-net/aspose.cells/range/merge/#) | Combine une plage de cellules en une seule cellule.|
| [un_merge()](/cells/fr/python-net/aspose.cells/range/un_merge/#) |Annule la fusion des cellules fusionnées de cette plage.|
| [put_value(string_value, is_converted, set_style)](/cells/fr/python-net/aspose.cells/range/put_value/#str-bool-bool) | Met une valeur dans la plage, le cas échéant, la valeur sera convertie en un autre type de données et le format numérique de la cellule sera réinitialisé.|
| [apply_style(style, flag)](/cells/fr/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) | Applique des formats pour toute une gamme.|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/fr/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) | Définir les bordures intérieures de la plage.|
| [move_to(dest_row, dest_column)](/cells/fr/python-net/aspose.cells/range/move_to/#int-int) | Déplacez la plage actuelle vers la plage de destination.|
| [copy_data(range)](/cells/fr/python-net/aspose.cells/range/copy_data/#Range) | Copie les données de cellule (y compris les formules) à partir d'une plage source.|
| [copy_value(range)](/cells/fr/python-net/aspose.cells/range/copy_value/#Range) | Copie la valeur de la cellule à partir d'une plage source.|
| [copy_style(range)](/cells/fr/python-net/aspose.cells/range/copy_style/#Range) | Copie les paramètres de style d'une plage source.|
| [get_cell_or_null(row_offset, column_offset)](/cells/fr/python-net/aspose.cells/range/get_cell_or_null/#int-int) | Obtient [Cell](/cells/fr/python-net/aspose.cells/cell) objet ou null dans cette plage.|
| [get_offset(row_offset, column_offset)](/cells/fr/python-net/aspose.cells/range/get_offset/#int-int) | Obtient la plage [Range](/cells/fr/python-net/aspose.cells/range) par décalage.|



###  Exemple

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

###  Voir également
* module [aspose.cells](..)
* classe [Cell](/cells/fr/python-net/aspose.cells/cell)
* classe [Range](/cells/fr/python-net/aspose.cells/range)
