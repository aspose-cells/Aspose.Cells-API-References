---
title: PivotFilter classe
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.pivot/pivotfilter/
is_root: false
---
##  PivotFilter classe
Représente un PivotFilter dans la collection PivotFilter.



Le type PivotFilter expose les membres suivants :

###  Propriétés
| Propriété| Description|
| :- | :- |
| [auto_filter](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/auto_filter) | Obtient le filtre automatique du filtre pivot.|
| [filter_type](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/filter_type) | Obtient le type de filtre automatique du filtre pivot.|
| [field_index](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/field_index) |Obtient l'index de champ du filtre pivot.|
| [value1](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/value1) | Obtient la chaîne value1 du filtre de pivot d'étiquette.|
| [value2](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/value2) | Obtient la valeur de chaîne2 du filtre de pivot d'étiquette.|
| [measure_fld_index](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/measure_fld_index) | Obtient l'index de champ de mesure du filtre pivot.|
| [member_property_field_index](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/member_property_field_index) | Obtient l'index de champ de propriété de membre du filtre pivot.|
| [name](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/name) | Obtient le nom du filtre pivot.|
| [evaluation_order](/cells/fr/python-net/aspose.cells.pivot/pivotfilter/evaluation_order) | Obtient l'ordre d'évaluation du filtre pivot.|



###  Exemples

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType

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
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

###  Voir également
* module [aspose.cells.pivot](..)
