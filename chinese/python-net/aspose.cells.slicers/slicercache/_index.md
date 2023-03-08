---
title: SlicerCache类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.slicers/slicercache/
is_root: false
---
##  SlicerCache类
切片器缓存的简要说明



SlicerCache 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [cross_filter_type](/cells/zh/python-net/aspose.cells.slicers/slicercache/cross_filter_type) |返回或设置切片器是否参与与其他切片器的交叉过滤<br/>共享相同的切片器缓存，以及如何显示交叉过滤。读/写|
| [list](/cells/zh/python-net/aspose.cells.slicers/slicercache/list) |返回与指定切片器缓存关联的切片器是否基于非 OLAP 数据源。只读|
| [slicer_cache_items](/cells/zh/python-net/aspose.cells.slicers/slicercache/slicer_cache_items) |返回一个 SlicerCacheItem 集合，其中包含切片器缓存中所有项目的集合。只读|
| [name](/cells/zh/python-net/aspose.cells.slicers/slicercache/name) |返回切片器缓存的名称。|
| [source_name](/cells/zh/python-net/aspose.cells.slicers/slicercache/source_name) |返回缓存字段的名称|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from aspose.cells.slicers import SlicerStyleType

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
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
slicerIndex = slicers.add(pivot, "E12", "fruit")
slicer = slicers[slicerIndex]
slicer.style_type = SlicerStyleType.SLICER_STYLE_LIGHT2
# Get SlicerCache object of current slicer
slicerCache = slicer.slicer_cache
# do your business
book.save("out.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.slicers](..)
