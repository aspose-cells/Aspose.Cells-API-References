---
title: PivotFilter类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.pivot/pivotfilter/
is_root: false
---
## PivotFilter类
代表 PivotFilter 集合中的 PivotFilter。



PivotFilter 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [auto_filter](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/auto_filter) |获取数据透视过滤器的自动过滤器。|
| [filter_type](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/filter_type) |获取数据透视过滤器的自动过滤器类型。|
| [field_index](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/field_index) |获取数据透视过滤器的字段索引。|
| [value1](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/value1) |获取标签数据透视过滤器的字符串 value1。|
| [value2](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/value2) |获取标签数据透视过滤器的字符串值 2。|
| [measure_fld_index](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/measure_fld_index) |获取数据透视过滤器的度量字段索引。|
| [member_property_field_index](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/member_property_field_index) |获取数据透视过滤器的成员属性字段索引。|
| [name](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/name) |获取数据透视过滤器的名称。|
| [evaluation_order](/cells/zh/python-net/aspose.cells.pivot/pivotfilter/evaluation_order) |获取数据透视过滤器的评估顺序。|



### 例子

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

### 也可以看看
* 模块 [aspose.cells.pivot](..)
