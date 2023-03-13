---
title: CellsHelper classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 230
url: /fr/python-net/aspose.cells/cellshelper/
is_root: false
---
##  CellsHelper classe
Fournit des fonctions d'assistance.



Le type CellsHelper expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [significant_digits](/cells/fr/python-net/aspose.cells/cellshelper/significant_digits) | Obtient et définit le nombre de chiffres significatifs.<br/> La valeur par défaut est 17.|
| [dpi](/cells/fr/python-net/aspose.cells/cellshelper/dpi) | Obtient le DPI de la machine.|
| [startup_path](/cells/fr/python-net/aspose.cells/cellshelper/startup_path) |Obtient ou définit le chemin de démarrage, auquel font référence certaines références de formules externes.|
| [alt_start_path](/cells/fr/python-net/aspose.cells/cellshelper/alt_start_path) | Obtient ou définit le chemin de démarrage alternatif, auquel font référence certaines références de formules externes.|
| [library_path](/cells/fr/python-net/aspose.cells/cellshelper/library_path) | Obtient ou définit le chemin d'accès à la bibliothèque auquel font référence certaines références de formule externes.|
| [custom_implementation_factory](/cells/fr/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Obtient ou définit la fabrique pour créer des instances avec une implémentation spéciale.|
| [is_cloud_platform](/cells/fr/python-net/aspose.cells/cellshelper/is_cloud_platform) | Veuillez définir cette propriété sur True lors de l'exécution sur une plate-forme cloud, telle que : Azure, AWSLambda, etc.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/fr/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Vérifie le nom de la feuille donnée et en crée une valide si nécessaire.<br/>Si le nom de feuille donné est conforme aux règles du nom de feuille Excel, renvoyez-le.<br/>Sinon, la chaîne sera tronquée si la longueur dépasse la limite<br/> et les caractères invalides seront remplacés par ' ', puis renvoient la valeur de chaîne reconstruite.|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/fr/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Vérifie le nom de la feuille donnée et en crée une valide si nécessaire.<br/>Si le nom de feuille donné est conforme aux règles du nom de feuille Excel, renvoyez-le.<br/>Sinon, la chaîne sera tronquée si la longueur dépasse la limite<br/> et les caractères invalides seront remplacés par le caractère donné, puis renverront la valeur de chaîne reconstruite.|
| [get_text_width(text, font, scaling)](/cells/fr/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Obtenir la largeur du texte en unité de points.|
| [get_version()](/cells/fr/python-net/aspose.cells/cellshelper/get_version/#) | Obtenez la version finale.|
| [cell_name_to_index(cell_name, row, column)](/cells/fr/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Obtient les index de ligne et de colonne de cellule en fonction de son nom.|
| [cell_index_to_name(row, column)](/cells/fr/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Obtient le nom de la cellule en fonction de ses index de ligne et de colonne.|
| [column_index_to_name(column)](/cells/fr/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Obtient le nom de la colonne en fonction de l'index de la colonne.|
| [column_name_to_index(column_name)](/cells/fr/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |Obtient l'index de la colonne en fonction du nom de la colonne.|
| [row_index_to_name(row)](/cells/fr/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Obtient le nom de la ligne en fonction de l'index de la ligne.|
| [row_name_to_index(row_name)](/cells/fr/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Obtient l'index de ligne en fonction du nom de la ligne.|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/fr/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Convertit la formule r1c1 de la cellule en formule A1.|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/fr/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Convertit la formule A1 de la cellule en formule r1c1.|
| [get_date_time_from_double(double_value, date1904)](/cells/fr/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Convertissez la valeur double en valeur date/heure.|
| [get_double_from_date_time(date_time, date1904)](/cells/fr/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Convertir la date et l'heure en valeur double.|
| [get_used_colors(workbook)](/cells/fr/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Obtient toutes les couleurs utilisées dans le classeur.|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/fr/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Ajouter une fonction complémentaire.|
| [merge_files(files, cached_file, dest_file)](/cells/fr/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Fusionne certains fichiers xls volumineux dans un fichier xls.|
| [init_for_dot_net_core()](/cells/fr/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | Effectuez l'initialisation du programme .NetCore.<br/> Nous vous suggérons d'appeler cette méthode pour toutes les initialisations .NetCore en premier.<br/>Par exemple:<br/>CellsHelper.InitForDotNetCore();<br/> Workbook wb = new Workbook();|



###  Voir également
* module [aspose.cells](..)
