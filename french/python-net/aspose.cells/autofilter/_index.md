---
title: AutoFilter classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 70
url: /fr/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter classe
Représente le filtrage automatique pour la feuille de calcul spécifiée.



Le type AutoFilter expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [sorter](/cells/fr/python-net/aspose.cells/autofilter/sorter) | Obtient le trieur de données.|
| [range](/cells/fr/python-net/aspose.cells/autofilter/range) | Représente la plage à laquelle s'applique le filtre automatique spécifié.|
| [show_filter_button](/cells/fr/python-net/aspose.cells/autofilter/show_filter_button) | Indique si le bouton Filtre automatique de cette colonne est visible.|
| [filter_columns](/cells/fr/python-net/aspose.cells/autofilter/filter_columns) | Obtient la collection des colonnes de filtre.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/fr/python-net/aspose.cells/autofilter/remove_filter/#int-str) | Supprime un filtre pour une colonne de filtre.|
| [remove_filter(field_index)](/cells/fr/python-net/aspose.cells/autofilter/remove_filter/#int) | Supprimez le filtre spécifique.|
| [custom(field_index, operator_type1, criteria1)](/cells/fr/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) | Filtre une liste avec un critère personnalisé.|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/fr/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) | Filtre une liste avec des critères personnalisés.|
| [refresh()](/cells/fr/python-net/aspose.cells/autofilter/refresh/#) | Actualisez les filtres automatiques pour masquer ou afficher les lignes.|
| [refresh(hide_rows)](/cells/fr/python-net/aspose.cells/autofilter/refresh/#bool) | Obtient tous les index des lignes masquées.|
| [set_range(row, start_column, end_column)](/cells/fr/python-net/aspose.cells/autofilter/set_range/#int-int-int) | Définit la plage à laquelle s'applique le filtre automatique spécifié.|
| [get_cell_area()](/cells/fr/python-net/aspose.cells/autofilter/get_cell_area/#) | Obtient le [CellArea](/cells/fr/python-net/aspose.cells/cellarea) auquel s'applique le filtre automatique spécifié.|
| [add_filter(field_index, criteria)](/cells/fr/python-net/aspose.cells/autofilter/add_filter/#int-str) | Ajoute un filtre pour une colonne de filtre.|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/fr/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Ajoute un filtre de date.|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/fr/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) | Supprime un filtre de date.|
| [filter(field_index, criteria)](/cells/fr/python-net/aspose.cells/autofilter/filter/#int-str) |Filtre une liste avec des critères spécifiés.|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/fr/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) | Filtrer les 10 premiers éléments de la liste|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/fr/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) | Ajoute un filtre dynamique.|
| [add_font_color_filter(field_index, color)](/cells/fr/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) | Ajoute un filtre de couleur de police.|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/fr/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) | Ajoute un filtre de couleur de remplissage.|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/fr/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) | Ajoute un filtre d'icônes.|
| [match_blanks(field_index)](/cells/fr/python-net/aspose.cells/autofilter/match_blanks/#int) | Faites correspondre toutes les cellules vides de la liste.|
| [match_non_blanks(field_index)](/cells/fr/python-net/aspose.cells/autofilter/match_non_blanks/#int) | Faites correspondre toutes les cellules non vides de la liste.|
| [show_all()](/cells/fr/python-net/aspose.cells/autofilter/show_all/#) | Afficher toutes les lignes.|



###  Exemple

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

###  Voir également
* module [aspose.cells](..)
* classe [CellArea](/cells/fr/python-net/aspose.cells/cellarea)
