---
title: Slicer类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.slicers/slicer/
is_root: false
---
##  Slicer类
Slicer视图的概要描述



Slicer 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [title](/cells/zh/python-net/aspose.cells.slicers/slicer/title) |指定当前切片器对象的标题。|
| [alternative_text](/cells/zh/python-net/aspose.cells.slicers/slicer/alternative_text) |返回或设置 Slicer 对象的描述性（替代）文本字符串。|
| [is_printable](/cells/zh/python-net/aspose.cells.slicers/slicer/is_printable) |指示切片器对象是否可打印。|
| [is_locked](/cells/zh/python-net/aspose.cells.slicers/slicer/is_locked) |指示切片器形状是否已锁定。|
| [placement](/cells/zh/python-net/aspose.cells.slicers/slicer/placement) |表示绘图对象附加到其下方单元格的方式。<br/>该属性控制对象在工作表上的位置。|
| [locked_aspect_ratio](/cells/zh/python-net/aspose.cells.slicers/slicer/locked_aspect_ratio) |指示是否锁定纵横比。|
| [locked_position](/cells/zh/python-net/aspose.cells.slicers/slicer/locked_position) |指示是否可以使用用户界面移动或调整指定切片器的大小。|
| [slicer_cache](/cells/zh/python-net/aspose.cells.slicers/slicer/slicer_cache) |返回与切片器关联的 SlicerCache 对象。只读。|
| [parent](/cells/zh/python-net/aspose.cells.slicers/slicer/parent) |返回代表包含切片器的工作表的 Worksheet 对象。只读。|
| [style_type](/cells/zh/python-net/aspose.cells.slicers/slicer/style_type) |指定内置切片器样式的类型<br/>默认类型是 SlicerStyleLight1|
| [name](/cells/zh/python-net/aspose.cells.slicers/slicer/name) |返回或设置指定切片器的名称|
| [caption](/cells/zh/python-net/aspose.cells.slicers/slicer/caption) |返回或设置指定切片器的标题。|
| [caption_visible](/cells/zh/python-net/aspose.cells.slicers/slicer/caption_visible) |返回或设置显示切片器 Caption 的标题是否可见<br/>默认值是true|
| [number_of_columns](/cells/zh/python-net/aspose.cells.slicers/slicer/number_of_columns) |返回或设置指定切片器中的列数。|
| [left_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/left_pixel) |返回或设置切片器形状与其左列的水平偏移量（以像素为单位）。|
| [top_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/top_pixel) |返回或设置切片器形状与其顶行的垂直偏移量（以像素为单位）。|
| [width](/cells/zh/python-net/aspose.cells.slicers/slicer/width) |返回或设置指定切片器的宽度，以磅为单位。|
| [width_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/width_pixel) |返回或设置指定切片器的宽度，以像素为单位。|
| [height](/cells/zh/python-net/aspose.cells.slicers/slicer/height) |返回或设置指定切片器的高度，以磅为单位。|
| [height_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/height_pixel) |返回或设置指定切片器的高度，以像素为单位。|
| [column_width_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/column_width_pixel) |获取或设置切片器每列的宽度（以像素为单位）。|
| [column_width](/cells/zh/python-net/aspose.cells.slicers/slicer/column_width) |返回或设置切片器中每列的宽度（以磅为单位）。|
| [row_height_pixel](/cells/zh/python-net/aspose.cells.slicers/slicer/row_height_pixel) |返回或设置指定切片器中每行的高度（以像素为单位）。|
| [row_height](/cells/zh/python-net/aspose.cells.slicers/slicer/row_height) |返回或设置指定切片器中每行的高度（以磅为单位）。|


### 方法
|方法|描述|
| :- | :- |
| [add_pivot_connection(pivot)](/cells/zh/python-net/aspose.cells.slicers/slicer/add_pivot_connection/#aspose.cells.pivot.PivotTable) |添加数据透视表连接。|
| [remove_pivot_connection(pivot)](/cells/zh/python-net/aspose.cells.slicers/slicer/remove_pivot_connection/#aspose.cells.pivot.PivotTable) |删除数据透视表连接。|
| [refresh()](/cells/zh/python-net/aspose.cells.slicers/slicer/refresh/#) |刷新切片器。同时，刷新和计算相关数据透视表。|



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
items = slicer.slicer_cache.slicer_cache_items
item = items[0]
item.selected = False
# do your business
book.save("out.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.slicers](..)
