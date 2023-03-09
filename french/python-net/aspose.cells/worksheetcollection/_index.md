---
title: WorksheetCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1630
url: /fr/python-net/aspose.cells/worksheetcollection/
is_root: false
---
##  WorksheetCollection classe
Encapsule une collection de [Worksheet](/cells/fr/python-net/aspose.cells/worksheet) objets.



Le type WorksheetCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [web_extension_task_panes](/cells/fr/python-net/aspose.cells/worksheetcollection/web_extension_task_panes) | Obtient la liste des volets Office.|
| [web_extensions](/cells/fr/python-net/aspose.cells/worksheetcollection/web_extensions) | Obtient la liste des volets Office.|
| [threaded_comment_authors](/cells/fr/python-net/aspose.cells/worksheetcollection/threaded_comment_authors) | Obtient la liste des auteurs de commentaires thématiques.|
| [is_refresh_all_connections](/cells/fr/python-net/aspose.cells/worksheetcollection/is_refresh_all_connections) | Indique si toutes les connexions sont actualisées à l'ouverture du fichier dans MS Excel.|
| [names](/cells/fr/python-net/aspose.cells/worksheetcollection/names) | Obtient la collection de tous les objets Name de la feuille de calcul.|
| [active_sheet_name](/cells/fr/python-net/aspose.cells/worksheetcollection/active_sheet_name) | Représente le nom de la feuille de calcul active lorsque la feuille de calcul est ouverte.|
| [active_sheet_index](/cells/fr/python-net/aspose.cells/worksheetcollection/active_sheet_index) | Représente l'index de la feuille de calcul active lorsque la feuille de calcul est ouverte.|
| [dxfs](/cells/fr/python-net/aspose.cells/worksheetcollection/dxfs) | Obtient les enregistrements principaux de mise en forme différentielle.|
| [xml_maps](/cells/fr/python-net/aspose.cells/worksheetcollection/xml_maps) | Obtient et définit les mappages XML dans le classeur.|
| [built_in_document_properties](/cells/fr/python-net/aspose.cells/worksheetcollection/built_in_document_properties) | Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document intégrées de la feuille de calcul.|
| [custom_document_properties](/cells/fr/python-net/aspose.cells/worksheetcollection/custom_document_properties) | Renvoie une collection [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty) qui représente toutes les propriétés de document personnalisées de la feuille de calcul.|
| [ole_size](/cells/fr/python-net/aspose.cells/worksheetcollection/ole_size) | Obtient et définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole.|
| [external_links](/cells/fr/python-net/aspose.cells/worksheetcollection/external_links) | Représente des liens externes dans un classeur.|
| [table_styles](/cells/fr/python-net/aspose.cells/worksheetcollection/table_styles) | Obtient l'objet [WorksheetCollection.table_styles](/cells/fr/python-net/aspose.cells/worksheetcollection#table_styles).|
| [revision_logs](/cells/fr/python-net/aspose.cells/worksheetcollection/revision_logs) | Représente les journaux de révision.|
| [capacity](/cells/fr/python-net/aspose.cells/worksheetcollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [get(index)](/cells/fr/python-net/aspose.cells/worksheetcollection/get/#int) | Ajouter API for Python Via .Net.car cet [int index] n'est pas pris en charge|
| [get(sheet_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/get/#str) | Ajouter API for Python Via .Net.puisque cette [string sheetName] n'est pas prise en charge|
| [add(type)](/cells/fr/python-net/aspose.cells/worksheetcollection/add/#SheetType) | Ajoute une feuille de calcul à la collection.|
| [add()](/cells/fr/python-net/aspose.cells/worksheetcollection/add/#) | Ajoute une feuille de calcul à la collection.|
| [add(sheet_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/add/#str) | Ajoute une feuille de calcul à la collection.|
| [register_add_in_function(add_in_file, function_name, lib)](/cells/fr/python-net/aspose.cells/worksheetcollection/register_add_in_function/#str-str-bool) | Ajoute une fonction complémentaire dans le classeur|
| [register_add_in_function(id, function_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/register_add_in_function/#int-str) | Ajoute une fonction complémentaire dans le classeur|
| [add_copy(sheet_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/add_copy/#str) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.|
| [add_copy(sheet_index)](/cells/fr/python-net/aspose.cells/worksheetcollection/add_copy/#int) | Ajoute une feuille de calcul à la collection et copie les données d'une feuille de calcul existante.|
| [get_range_by_name(range_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str) | Obtient l'objet Range par nom prédéfini.|
| [get_range_by_name(range_name, current_sheet_index, include_table)](/cells/fr/python-net/aspose.cells/worksheetcollection/get_range_by_name/#str-int-bool) | Obtient [Range](/cells/fr/python-net/aspose.cells/range) par nom prédéfini ou nom de table|
| [copy_to(array)](/cells/fr/python-net/aspose.cells/worksheetcollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells/worksheetcollection/copy_to/#int-list-int-int) | Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells/worksheetcollection/index_of/#Worksheet-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells/worksheetcollection/last_index_of/#Worksheet-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [create_range(address, sheet_index)](/cells/fr/python-net/aspose.cells/worksheetcollection/create_range/#str-int) | Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir d'une adresse de la plage.|
| [create_union_range(address, sheet_index)](/cells/fr/python-net/aspose.cells/worksheetcollection/create_union_range/#str-int) | Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir d'une adresse de la plage.|
| [get_sheet_by_code_name(code_name)](/cells/fr/python-net/aspose.cells/worksheetcollection/get_sheet_by_code_name/#str) | Obtient la feuille de calcul par le nom de code.|
| [sort_names()](/cells/fr/python-net/aspose.cells/worksheetcollection/sort_names/#) | Trie les noms définis.|
| [swap_sheet(sheet_index1, sheet_index2)](/cells/fr/python-net/aspose.cells/worksheetcollection/swap_sheet/#int-int) | Intervertit les deux feuilles.|
| [remove_at(name)](/cells/fr/python-net/aspose.cells/worksheetcollection/remove_at/#str) | Supprime l'élément à un nom spécifié.|
| [get_named_ranges()](/cells/fr/python-net/aspose.cells/worksheetcollection/get_named_ranges/#) | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul.|
| [get_named_ranges_and_tables()](/cells/fr/python-net/aspose.cells/worksheetcollection/get_named_ranges_and_tables/#) | Obtient toutes les plages nommées prédéfinies dans la feuille de calcul.|
| [set_ole_size(start_row, end_row, start_column, end_column)](/cells/fr/python-net/aspose.cells/worksheetcollection/set_ole_size/#int-int-int-int) | Définit la taille affichée lorsque le fichier Workbook est utilisé comme objet Ole.|
| [clear_pivottables()](/cells/fr/python-net/aspose.cells/worksheetcollection/clear_pivottables/#) | Efface les tableaux croisés dynamiques de la feuille de calcul.|
| [refresh_pivot_tables()](/cells/fr/python-net/aspose.cells/worksheetcollection/refresh_pivot_tables/#) |Actualise tous les tableaux croisés dynamiques dans WorksheetCollection.|
| [binary_search(item)](/cells/fr/python-net/aspose.cells/worksheetcollection/binary_search/#Worksheet) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



###  Exemple

```python
from aspose.cells import Workbook

workbook = Workbook()
sheets = workbook.worksheets
# Add a worksheet
sheets.add()
# Change the name of a worksheet
sheets[0].name = "First Sheet"
# Set the active sheet to the second worksheet
sheets.active_sheet_index = 1

```

###  Voir également
* module [aspose.cells](..)
* classe [DocumentProperty](/cells/fr/python-net/aspose.cells.properties/documentproperty)
* classe [Range](/cells/fr/python-net/aspose.cells/range)
* classe [Worksheet](/cells/fr/python-net/aspose.cells/worksheet)
