---
title: PivotTable classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 100
url: /fr/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  PivotTable classe
Description sommaire pour PivotTable.



Le type PivotTable expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [is_excel_2003_compatible](/cells/fr/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) | Spécifie si le tableau croisé dynamique est compatible avec Excel2003 lors de l'actualisation du tableau croisé dynamique,<br/>si vrai, une chaîne doit être inférieure ou égale à 255 caractères, donc si la chaîne est supérieure à 255 caractères,<br/>il sera tronqué. si false, une chaîne n'aura pas la restriction susmentionnée.<br/> La valeur par défaut est true.|
| [refreshed_by_who](/cells/fr/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) | Obtient le nom de l'utilisateur qui a actualisé le tableau croisé dynamique pour la dernière fois|
| [refresh_date](/cells/fr/python-net/aspose.cells.pivot/pivottable/refresh_date) | Obtient la date à laquelle le tableau croisé dynamique a été actualisé pour la dernière fois.|
| [pivot_table_style_name](/cells/fr/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) | Obtient et définit le nom du style de tableau croisé dynamique.|
| [pivot_table_style_type](/cells/fr/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) | Obtient et définit le style de tableau croisé dynamique intégré.|
| [column_fields](/cells/fr/python-net/aspose.cells.pivot/pivottable/column_fields) | Renvoie un objet PivotFields actuellement affiché sous forme de champs de colonne.|
| [row_fields](/cells/fr/python-net/aspose.cells.pivot/pivottable/row_fields) | Renvoie un objet PivotFields actuellement affiché sous forme de champs de ligne.|
| [page_fields](/cells/fr/python-net/aspose.cells.pivot/pivottable/page_fields) | Renvoie un objet PivotFields actuellement affiché en tant que champs de page.|
| [data_fields](/cells/fr/python-net/aspose.cells.pivot/pivottable/data_fields) | Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique.<br/>Lecture seule. Ce serait init uniquement lorsqu'il y a deux champs de données ou plus dans DataPiovtFiels.<br/>Il sert uniquement à ajouter DataPivotField à la zone de ligne/colonne du tableau croisé dynamique. La valeur par défaut est dans la zone de ligne.|
| [data_field](/cells/fr/python-net/aspose.cells.pivot/pivottable/data_field) | Obtient un objet PivotField qui représente tous les champs de données d'un tableau croisé dynamique.<br/>Lecture seule. Ce serait init uniquement lorsqu'il y a deux champs de données ou plus dans DataPiovtFiels.<br/>Il sert uniquement à ajouter DataPivotField à la zone de ligne/colonne du tableau croisé dynamique. La valeur par défaut est dans la zone de ligne.|
| [base_fields](/cells/fr/python-net/aspose.cells.pivot/pivottable/base_fields) | Renvoie un objet PivotFields qui inclut tous les champs du rapport de tableau croisé dynamique|
| [pivot_filters](/cells/fr/python-net/aspose.cells.pivot/pivottable/pivot_filters) | Renvoie un objet PivotFilterCollection.|
| [column_range](/cells/fr/python-net/aspose.cells.pivot/pivottable/column_range) | Renvoie un objet CellArea qui représente la plage<br/> qui contient la zone de colonne dans le rapport de tableau croisé dynamique. Lecture seulement.|
| [row_range](/cells/fr/python-net/aspose.cells.pivot/pivottable/row_range) | Renvoie un objet CellArea qui représente la plage<br/> qui contient la zone de ligne dans le rapport de tableau croisé dynamique. Lecture seulement.|
| [data_body_range](/cells/fr/python-net/aspose.cells.pivot/pivottable/data_body_range) | Renvoie un objet CellArea qui représente la plage contenant la zone de données<br/> dans la liste entre la ligne d'en-tête et la ligne d'insertion. Lecture seulement.|
| [table_range1](/cells/fr/python-net/aspose.cells.pivot/pivottable/table_range1) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique,<br/> mais n'inclut pas les champs de page. Lecture seulement.|
| [table_range2](/cells/fr/python-net/aspose.cells.pivot/pivottable/table_range2) | Renvoie un objet CellArea qui représente la plage contenant l'intégralité du rapport de tableau croisé dynamique,<br/> inclut des champs de page. Lecture seulement.|
| [column_grand](/cells/fr/python-net/aspose.cells.pivot/pivottable/column_grand) | Indique si le rapport de tableau croisé dynamique affiche les totaux généraux pour les colonnes.|
| [is_grid_drop_zones](/cells/fr/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) | Indique si le rapport de tableau croisé dynamique affiche une disposition de tableau croisé dynamique classique.<br/> (permet de faire glisser des champs dans la grille)|
| [row_grand](/cells/fr/python-net/aspose.cells.pivot/pivottable/row_grand) |Indique si le rapport de tableau croisé dynamique affiche les totaux généraux pour les lignes.|
| [display_null_string](/cells/fr/python-net/aspose.cells.pivot/pivottable/display_null_string) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée<br/> dans les cellules contenant des valeurs nulles.|
| [null_string](/cells/fr/python-net/aspose.cells.pivot/pivottable/null_string) | Obtient la chaîne affichée dans les cellules contenant des valeurs nulles<br/> lorsque la propriété DisplayNullString est vraie. La valeur par défaut est une chaîne vide.|
| [display_error_string](/cells/fr/python-net/aspose.cells.pivot/pivottable/display_error_string) | Indique si le rapport de tableau croisé dynamique affiche une chaîne personnalisée dans les cellules contenant des erreurs.|
| [data_field_header_name](/cells/fr/python-net/aspose.cells.pivot/pivottable/data_field_header_name) | Obtient et définit le nom de l'en-tête de champ de la zone de valeur dans le tableau croisé dynamique.|
| [error_string](/cells/fr/python-net/aspose.cells.pivot/pivottable/error_string) | Obtient la chaîne affichée dans les cellules contenant des erreurs<br/> lorsque la propriété DisplayErrorString est vraie. La valeur par défaut est une chaîne vide.|
| [is_auto_format](/cells/fr/python-net/aspose.cells.pivot/pivottable/is_auto_format) | Indique si le rapport de tableau croisé dynamique est automatiquement formaté.<br/>Case à cocher "tableau format automatique" qui est dans l'option tableau croisé dynamique pour Excel 2003<br/> Case à cocher "Autofit column width on update" qui se trouve dans les options du tableau croisé dynamique :Format de mise en page pour Excel 2007|
| [auto_format_type](/cells/fr/python-net/aspose.cells.pivot/pivottable/auto_format_type) | Obtient le type de format automatique de tableau croisé dynamique.|
| [has_blank_rows](/cells/fr/python-net/aspose.cells.pivot/pivottable/has_blank_rows) | Indique s'il faut ajouter des lignes vides.<br/>Cette propriété s'applique uniquement aux types de format automatique de tableau croisé dynamique qui doivent ajouter des lignes vides.|
| [merge_labels](/cells/fr/python-net/aspose.cells.pivot/pivottable/merge_labels) | Indique si l'élément de ligne externe, l'élément de colonne, le sous-total,<br/> et les étiquettes de total général utilisent des cellules fusionnées.|
| [preserve_formatting](/cells/fr/python-net/aspose.cells.pivot/pivottable/preserve_formatting) | Indique si la mise en forme est conservée lorsque le tableau croisé dynamique est actualisé ou recalculé.|
| [show_drill](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_drill) | Obtient si les boutons développer/réduire sont affichés.|
| [enable_drilldown](/cells/fr/python-net/aspose.cells.pivot/pivottable/enable_drilldown) | Obtient si l'exploration est activée.|
| [enable_field_dialog](/cells/fr/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) | Indique si la boîte de dialogue Champ de tableau croisé dynamique est disponible<br/> lorsque l'utilisateur double-clique sur le champ Tableau croisé dynamique.|
| [enable_field_list](/cells/fr/python-net/aspose.cells.pivot/pivottable/enable_field_list) | Obtient si activer la liste de champs pour le tableau croisé dynamique.|
| [enable_wizard](/cells/fr/python-net/aspose.cells.pivot/pivottable/enable_wizard) | Indique si l'Assistant Tableau croisé dynamique est disponible.|
| [subtotal_hidden_page_items](/cells/fr/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) | Indique si les éléments de champ de page masqués dans le rapport de tableau croisé dynamique<br/>sont inclus dans les sous-totaux de ligne et de colonne, les totaux de bloc et les totaux généraux.<br/> La valeur par défaut est Faux.|
| [grand_total_name](/cells/fr/python-net/aspose.cells.pivot/pivottable/grand_total_name) | Renvoie l'étiquette de chaîne de texte affichée dans l'en-tête de colonne ou de ligne du total général.<br/> La valeur par défaut est la chaîne "Grand Total".|
| [manual_update](/cells/fr/python-net/aspose.cells.pivot/pivottable/manual_update) |Indique si le rapport de tableau croisé dynamique est recalculé uniquement à la demande de l'utilisateur.|
| [is_multiple_field_filters](/cells/fr/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres définis sur eux.|
| [missing_items_limit](/cells/fr/python-net/aspose.cells.pivot/pivottable/missing_items_limit) | Spécifie une valeur booléenne qui indique si les champs d'un tableau croisé dynamique peuvent avoir plusieurs filtres définis sur eux.|
| [enable_data_value_editing](/cells/fr/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) | Spécifie une valeur booléenne qui indique si l'utilisateur est autorisé à modifier les cellules dans la zone de données du tableau croisé dynamique.<br/> Activer la modification des cellules dans la zone des valeurs|
| [show_data_tips](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_data_tips) | Spécifie une valeur booléenne qui indique si les info-bulles doivent être affichées pour les cellules de données de tableau croisé dynamique.|
| [show_member_property_tips](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) | Spécifie une valeur booléenne qui indique si les informations de propriété de membre doivent être omises des info-bulles de tableau croisé dynamique.|
| [show_values_row](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_values_row) | Spécifie une valeur booléenne qui indique si afficher la ligne des valeurs.<br/> afficher la ligne des valeurs|
| [show_empty_col](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_empty_col) | Spécifie une valeur booléenne qui indique s'il faut inclure des colonnes vides dans le tableau|
| [show_empty_row](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_empty_row) | Spécifie une valeur booléenne qui indique s'il faut inclure des lignes vides dans le tableau.|
| [field_list_sort_ascending](/cells/fr/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) |Spécifie une valeur booléenne qui indique si les champs du tableau croisé dynamique sont triés dans un ordre autre que celui par défaut dans la liste des champs.|
| [print_drill](/cells/fr/python-net/aspose.cells.pivot/pivottable/print_drill) | Spécifie une valeur booléenne qui indique si les indicateurs d'exploration doivent être imprimés.<br/> imprimer les boutons développer/réduire lorsqu'ils sont affichés sur le tableau croisé dynamique.|
| [alt_text_title](/cells/fr/python-net/aspose.cells.pivot/pivottable/alt_text_title) | Obtient le titre de l'altertext|
| [alt_text_description](/cells/fr/python-net/aspose.cells.pivot/pivottable/alt_text_description) | Obtient la description du texte alternatif|
| [name](/cells/fr/python-net/aspose.cells.pivot/pivottable/name) | Obtient le nom du tableau croisé dynamique|
| [column_header_caption](/cells/fr/python-net/aspose.cells.pivot/pivottable/column_header_caption) | Obtient la légende d'en-tête de colonne du tableau croisé dynamique.|
| [indent](/cells/fr/python-net/aspose.cells.pivot/pivottable/indent) | Spécifie l'incrément d'indentation pour l'axe compact et peut être utilisé pour définir la mise en page du rapport sur forme compacte.|
| [row_header_caption](/cells/fr/python-net/aspose.cells.pivot/pivottable/row_header_caption) | Obtient la légende d'en-tête de ligne du tableau croisé dynamique.|
| [show_row_header_caption](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) | Indique si la légende de l'en-tête de ligne est affichée dans le rapport de tableau croisé dynamique<br/> Indique si Afficher les légendes des champs et les listes déroulantes des filtres|
| [custom_list_sort](/cells/fr/python-net/aspose.cells.pivot/pivottable/custom_list_sort) | Indique si la liste personnalisée intégrée doit être prise en compte lors du tri des données|
| [pivot_format_conditions](/cells/fr/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) | Obtient les conditions de format du tableau croisé dynamique.|
| [page_field_order](/cells/fr/python-net/aspose.cells.pivot/pivottable/page_field_order) | Obtient l'ordre dans lequel les champs de page sont ajoutés à la disposition du rapport de tableau croisé dynamique.|
| [page_field_wrap_count](/cells/fr/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) |Obtient le nombre de champs de page dans chaque colonne ou ligne du rapport de tableau croisé dynamique.|
| [tag](/cells/fr/python-net/aspose.cells.pivot/pivottable/tag) | Obtient une chaîne enregistrée avec le rapport de tableau croisé dynamique.|
| [save_data](/cells/fr/python-net/aspose.cells.pivot/pivottable/save_data) | Indique si les données du rapport de tableau croisé dynamique sont enregistrées avec le classeur.|
| [refresh_data_on_opening_file](/cells/fr/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) | Indique si Actualiser les données lors de l'ouverture du fichier.|
| [refresh_data_flag](/cells/fr/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) | Indique si Actualiser les données ou non.|
| [external_connection_data_source](/cells/fr/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) | Obtient la source de données de connexion externe.|
| [data_source](/cells/fr/python-net/aspose.cells.pivot/pivottable/data_source) | Obtient et définit la source de données du tableau croisé dynamique.|
| [item_print_titles](/cells/fr/python-net/aspose.cells.pivot/pivottable/item_print_titles) | Un bit qui spécifie si les légendes des éléments de pivot sur l'axe des lignes<br/> sont répétés sur chaque page imprimée pour les champs pivot sous forme de tableau.|
| [print_titles](/cells/fr/python-net/aspose.cells.pivot/pivottable/print_titles) | Indique si les titres d'impression de la feuille de calcul sont définis en fonction<br/> sur le rapport de tableau croisé dynamique. La valeur par défaut est faux.|
| [display_immediate_items](/cells/fr/python-net/aspose.cells.pivot/pivottable/display_immediate_items) | Indique si les éléments des zones de ligne et de colonne sont visibles<br/> lorsque la zone de données du tableau croisé dynamique est vide. La valeur par défaut est true.|
| [is_selected](/cells/fr/python-net/aspose.cells.pivot/pivottable/is_selected) | Indique si le tableau croisé dynamique est sélectionné.|
| [show_pivot_style_row_header](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) | Indique si l'en-tête de ligne dans le tableau croisé dynamique doit avoir le style appliqué.|
| [show_pivot_style_column_header](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) |Indique si l'en-tête de colonne du tableau croisé dynamique doit avoir le style appliqué.|
| [show_pivot_style_row_stripes](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) | Indique si la mise en forme des bandes de ligne est appliquée.|
| [show_pivot_style_column_stripes](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) | Indique si la mise en forme des bandes de colonnes est appliquée.|
| [show_pivot_style_last_column](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) | Indique si la mise en forme des bandes de colonnes est appliquée.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/fr/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) | Supprime un champ d'une zone de champ spécifique|
| [remove_field(field_type, base_field_index)](/cells/fr/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) | Supprime un champ d'une zone de champ spécifique|
| [remove_field(field_type, pivot_field)](/cells/fr/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) | Supprimer le champ d'une zone de champ spécifique|
| [add_field_to_area(field_type, field_name)](/cells/fr/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) | Ajoute le champ à la zone spécifique.|
| [add_field_to_area(field_type, base_field_index)](/cells/fr/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) | Ajoute le champ à la zone spécifique.|
| [add_field_to_area(field_type, pivot_field)](/cells/fr/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) | Ajoute le champ à la zone spécifique.|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/fr/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) | Ajoute un champ calculé au champ pivot.|
| [add_calculated_field(name, formula)](/cells/fr/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) | Ajoute un champ calculé au champ pivot et faites-le glisser vers la zone de données.|
| [move(row, column)](/cells/fr/python-net/aspose.cells.pivot/pivottable/move/#int-int) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul.|
| [move(dest_cell_name)](/cells/fr/python-net/aspose.cells.pivot/pivottable/move/#str) | Déplace le tableau croisé dynamique vers un autre emplacement dans la feuille de calcul.|
| [set_auto_group_field(base_field_index)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) | Définit le groupe de champs automatique par le tableau croisé dynamique.|
| [set_auto_group_field(pivot_field)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) | Définit le groupe de champs automatique par le tableau croisé dynamique.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) | Définit le groupe de champs manuels par le tableau croisé dynamique.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) | Définit le groupe de champs manuels par le tableau croisé dynamique.|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) | Définit le groupe de champs manuels par le tableau croisé dynamique.|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) | Définit le groupe de champs manuels par le tableau croisé dynamique.|
| [set_ungroup(base_field_index)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) | Ensembles dégroupés par le tableau croisé dynamique|
| [set_ungroup(pivot_field)](/cells/fr/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) | Ensembles dégroupés par le tableau croisé dynamique|
| [copy_style(pivot_table)](/cells/fr/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) | Copie le style nommé d'un autre tableau croisé dynamique.|
| [show_report_filter_page(page_field)](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) | Afficher toutes les pages de filtre de rapport selon PivotField, le PivotField doit être situé dans les PageFields.|
| [show_report_filter_page_by_name(field_name)](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) | Afficher toutes les pages de filtre de rapport en fonction du nom de PivotField, le PivotField doit être situé dans les PageFields.|
| [show_report_filter_page_by_index(pos_index)](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) |Afficher toutes les pages de filtre de rapport en fonction de l'index de position dans les PageFields|
| [fields(field_type)](/cells/fr/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) | Obtient les champs spécifiques par le type de champ.|
| [change_data_source(source)](/cells/fr/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) | Définissez les données source du tableau croisé dynamique.<br/> Feuille1 !$A$1 :$C$3|
| [get_source()](/cells/fr/python-net/aspose.cells.pivot/pivottable/get_source/#) | Obtenez les données source de pivottable.|
| [refresh_data()](/cells/fr/python-net/aspose.cells.pivot/pivottable/refresh_data/#) | Actualise les données et les paramètres du tableau croisé dynamique à partir de sa source de données.|
| [calculate_data()](/cells/fr/python-net/aspose.cells.pivot/pivottable/calculate_data/#) | Calcule les données du tableau croisé dynamique dans les cellules.|
| [clear_data()](/cells/fr/python-net/aspose.cells.pivot/pivottable/clear_data/#) | Effacer les données et la mise en forme du tableau croisé dynamique|
| [calculate_range()](/cells/fr/python-net/aspose.cells.pivot/pivottable/calculate_range/#) | Calcule la plage du tableau croisé dynamique.|
| [format_all(style)](/cells/fr/python-net/aspose.cells.pivot/pivottable/format_all/#Style) | Formater toutes les cellules dans la zone de tableau croisé dynamique|
| [format_row(row, style)](/cells/fr/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) | Mettre en forme les données de ligne dans la zone de tableau croisé dynamique|
| [format(row, column, style)](/cells/fr/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) | Formater la cellule dans la zone de tableau croisé dynamique|
| [get_horizontal_breaks()](/cells/fr/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) | obtenir la liste d'index des lignes du tableau croisé dynamique des sauts de page horizontaux|
| [show_in_compact_form()](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) | Présente le tableau croisé dynamique sous une forme compacte.|
| [show_in_outline_form()](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) | Présente le tableau croisé dynamique sous forme de plan.|
| [show_in_tabular_form()](/cells/fr/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) | Présente le tableau croisé dynamique sous forme de tableau.|
| [get_cell_by_display_name(display_name)](/cells/fr/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) | Obtient l'objet Cell par le DisplayName de PivotField|
| [get_children()](/cells/fr/python-net/aspose.cells.pivot/pivottable/get_children/#) | Obtient les tableaux croisés dynamiques enfants qui utilisent ces données de tableau croisé dynamique comme source de données.|



###  Exemple

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Change PivotField's attributes
rowField = pivot.row_fields[0]
rowField.display_name = "custom display name"
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Voir également
* module [aspose.cells.pivot](..)
