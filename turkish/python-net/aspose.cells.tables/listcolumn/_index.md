---
title: ListColumn sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 10
url: /tr/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn sınıfı
Listedeki bir sütunu temsil eder.



ListColumn türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [name](/cells/tr/python-net/aspose.cells.tables/listcolumn/name) | Sütunun adını alır ve ayarlar.|
| [totals_calculation](/cells/tr/python-net/aspose.cells.tables/listcolumn/totals_calculation) | Liste sütununun Toplamlar satırındaki hesaplama türünü alır ve ayarlar.|
| [range](/cells/tr/python-net/aspose.cells.tables/listcolumn/range) | Bu liste sütununun aralığını alır.|
| [formula](/cells/tr/python-net/aspose.cells.tables/listcolumn/formula) | Liste sütununun formülünü alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | Bu liste sütununun toplam satırının formülünü alır.|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) | Bu liste sütununun toplam satırının formülünü alır.|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/tr/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | Bu liste sütununun formülünü alır.|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/tr/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) | Bu liste sütunu için formülü ayarlar.|



###  örnekler

```python
from aspose.cells import CellsHelper, Workbook
from aspose.cells.tables import TotalsCalculation

workbook = Workbook()
cells = workbook.worksheets[0].cells
for i in range(5):
    cells.get(0, i).put_value(CellsHelper.column_index_to_name(i))
for row in range(1, 10):
    for column in range(4):
        cells.get(row, column).put_value(row * column)
tables = workbook.worksheets[0].list_objects
index = tables.add(0, 0, 9, 4, True)
table = tables[0]
table.show_totals = True
listColumn = table.list_columns[4]
listColumn.totals_calculation = TotalsCalculation.SUM
listColumn.formula = "=[A]"
workbook.save(r"Book1.xlsx")

```

###  Ayrıca bakınız
* modül [aspose.cells.tables](..)
