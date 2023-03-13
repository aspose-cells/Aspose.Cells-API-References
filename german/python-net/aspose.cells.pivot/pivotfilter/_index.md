---
title: PivotFilter Klasse
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.pivot/pivotfilter/
is_root: false
---
##  PivotFilter Klasse
Stellt eine PivotFilter in der PivotFilter-Sammlung dar.



Der Typ PivotFilter macht die folgenden Member verfügbar:

###  Eigenschaften
| Eigentum| Beschreibung|
| :- | :- |
| [auto_filter](/cells/de/python-net/aspose.cells.pivot/pivotfilter/auto_filter) | Ruft den Autofilter des Pivot-Filters ab.|
| [filter_type](/cells/de/python-net/aspose.cells.pivot/pivotfilter/filter_type) | Ruft den Autofiltertyp des Pivotfilters ab.|
| [field_index](/cells/de/python-net/aspose.cells.pivot/pivotfilter/field_index) |Ruft den Feldindex des Pivot-Filters ab.|
| [value1](/cells/de/python-net/aspose.cells.pivot/pivotfilter/value1) | Ruft die Zeichenfolge value1 des Label-Pivot-Filters ab.|
| [value2](/cells/de/python-net/aspose.cells.pivot/pivotfilter/value2) | Ruft den Zeichenfolgenwert2 des Label-Pivot-Filters ab.|
| [measure_fld_index](/cells/de/python-net/aspose.cells.pivot/pivotfilter/measure_fld_index) | Ruft den Kennzahlenfeldindex des Pivot-Filters ab.|
| [member_property_field_index](/cells/de/python-net/aspose.cells.pivot/pivotfilter/member_property_field_index) | Ruft den Mitgliedseigenschaftsfeldindex des Pivotfilters ab.|
| [name](/cells/de/python-net/aspose.cells.pivot/pivotfilter/name) | Ruft den Namen des Pivot-Filters ab.|
| [evaluation_order](/cells/de/python-net/aspose.cells.pivot/pivotfilter/evaluation_order) | Ruft die Auswertungsreihenfolge des Pivot-Filters ab.|



###  Beispiel

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

###  Siehe auch
* Modul [aspose.cells.pivot](..)
