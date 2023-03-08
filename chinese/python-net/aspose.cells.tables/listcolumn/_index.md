---
title: ListColumn类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.tables/listcolumn/
is_root: false
---
##  ListColumn类
代表列表中的一列。



ListColumn 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [name](/cells/zh/python-net/aspose.cells.tables/listcolumn/name) |获取和设置列的名称。|
| [totals_calculation](/cells/zh/python-net/aspose.cells.tables/listcolumn/totals_calculation) |获取和设置列表列总计行中的计算类型。|
| [range](/cells/zh/python-net/aspose.cells.tables/listcolumn/range) |获取此列表列的范围。|
| [formula](/cells/zh/python-net/aspose.cells.tables/listcolumn/formula) |获取和设置列表列的公式。|


### 方法
|方法|描述|
| :- | :- |
| [get_custom_totals_row_formula(is_r1c1, is_local)](/cells/zh/python-net/aspose.cells.tables/listcolumn/get_custom_totals_row_formula/#bool-bool) |获取此列表列的总计行的公式。|
| [set_custom_totals_row_formula(formula, is_r1c1, is_local)](/cells/zh/python-net/aspose.cells.tables/listcolumn/set_custom_totals_row_formula/#str-bool-bool) |获取此列表列的总计行的公式。|
| [get_custom_calculated_formula(is_r1c1, is_local)](/cells/zh/python-net/aspose.cells.tables/listcolumn/get_custom_calculated_formula/#bool-bool) |获取此列表列的公式。|
| [set_custom_calculated_formula(formula, is_r1c1, is_local)](/cells/zh/python-net/aspose.cells.tables/listcolumn/set_custom_calculated_formula/#str-bool-bool) |设置此列表列的公式。|



### 例子

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

### 也可以看看
* 模块 [aspose.cells.tables](..)
