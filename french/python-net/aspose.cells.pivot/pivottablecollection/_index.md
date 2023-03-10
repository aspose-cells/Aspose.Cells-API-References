---
title: PivotTableCollection classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 110
url: /fr/python-net/aspose.cells.pivot/pivottablecollection/
is_root: false
---
##  PivotTableCollection classe
Représente la collection de tous les objets de tableau croisé dynamique sur la feuille de calcul spécifiée.



Le type PivotTableCollection expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [capacity](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/capacity) | Obtient ou définit le nombre d'éléments que la liste de tableau peut contenir.|


###  Méthodes
| Méthode| Description|
| :- | :- |
| [add(source_data, dest_cell_name, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str) | Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.|
| [add(source_data, dest_cell_name, table_name, use_same_source)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-str-str-bool) | Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.|
| [add(source_data, row, column, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str) | Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.|
| [add(source_data, row, column, table_name, use_same_source)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#str-int-int-str-bool) | Ajoute un nouveau cache de tableau croisé dynamique à une collection PivotCaches.|
| [add(pivot_table, dest_cell_name, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-str-str) | Ajoute un nouvel objet de tableau croisé dynamique à la collection à partir d'un autre tableau croisé dynamique.|
| [add(pivot_table, row, column, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#PivotTable-int-int-str) | Ajoute un nouvel objet de tableau croisé dynamique à la collection à partir d'un autre tableau croisé dynamique.|
| [add(source_data, is_auto_page, page_fields, dest_cell_name, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-str-str) | Ajoute un nouvel objet de tableau croisé dynamique à la collection avec plusieurs plages de consolidation comme source de données.|
| [add(source_data, is_auto_page, page_fields, row, column, table_name)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/add/#list-bool-PivotPageFields-int-int-str) | Ajoute un nouvel objet de tableau croisé dynamique à la collection avec plusieurs plages de consolidation comme source de données.|
| [copy_to(array)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#list) | Copie la totalité de la liste de tableaux dans une liste de tableaux unidimensionnelle compatible, en commençant au début de la liste de tableaux cible.|
| [copy_to(index, array, array_index, count)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/copy_to/#int-list-int-int) |Copie une plage d'éléments de la liste de tableaux vers une liste de tableaux unidimensionnelle compatible, en commençant à l'index spécifié de la liste de tableaux cible.|
| [index_of(item, index)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui s'étend de l'index spécifié au dernier élément.|
| [index_of(item, index, count)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/index_of/#PivotTable-int-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la première occurrence dans la plage d'éléments de la liste de tableaux qui commence à l'index spécifié et contient le nombre d'éléments spécifié.|
| [last_index_of(item)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la liste complète du tableau.|
| [last_index_of(item, index)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int) | Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui s'étend du premier élément à l'index spécifié.|
| [last_index_of(item, index, count)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/last_index_of/#PivotTable-int-int) |Recherche l'objet spécifié et renvoie l'index de base zéro de la dernière occurrence dans la plage d'éléments de la liste de tableaux qui contient le nombre d'éléments spécifié et se termine à l'index spécifié.|
| [remove_at(index, keep_data)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/remove_at/#int-bool) | Supprime le tableau croisé dynamique à l'index spécifié|
| [binary_search(item)](/cells/fr/python-net/aspose.cells.pivot/pivottablecollection/binary_search/#PivotTable) | Recherche un élément dans toute la liste de tableaux triés à l'aide du comparateur par défaut et renvoie l'index de base zéro de l'élément.|



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
