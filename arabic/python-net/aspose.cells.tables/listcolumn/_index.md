---
title: ListColumn الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 10
url: /ar/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn الدرجة
يمثل عمودًا في قائمة.



يكشف نوع ListColumn الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [name](/cells/ar/python-net/aspose.cells.tables/listcolumn/name) | الحصول على اسم العمود وتعيينه.|
| [totals_calculation](/cells/ar/python-net/aspose.cells.tables/listcolumn/totals_calculation) | الحصول على نوع الحساب وتعيينه في صف الإجماليات في عمود القائمة.|
| [range](/cells/ar/python-net/aspose.cells.tables/listcolumn/range) | يحصل على نطاق عمود القائمة هذا.|
| [formula](/cells/ar/python-net/aspose.cells.tables/listcolumn/formula) | الحصول على صيغة عمود القائمة وتعيينها.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) | يحصل على صيغة صف الإجماليات في عمود القائمة هذا.|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) | يحصل على صيغة صف الإجماليات في عمود القائمة هذا.|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/ar/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) | يحصل على صيغة عمود القائمة هذا.|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/ar/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) | يعيّن صيغة عمود القائمة هذا.|



###  مثال

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

###  أنظر أيضا
* وحدة [aspose.cells.tables](..)
