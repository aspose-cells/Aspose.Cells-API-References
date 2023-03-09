---
title: PivotField类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.pivot/pivotfield/
is_root: false
---
## PivotField类
表示数据透视表中的字段。



PivotField 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [pivot_items](/cells/zh/python-net/aspose.cells.pivot/pivotfield/pivot_items) |获取数据透视字段的数据透视项|
| [range](/cells/zh/python-net/aspose.cells.pivot/pivotfield/range) |获取数据透视字段的分组范围|
| [is_calculated_field](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_calculated_field) |指示指定的数据透视表字段是否为计算字段。|
| [base_index](/cells/zh/python-net/aspose.cells.pivot/pivotfield/base_index) |表示基础 PivotFields 中的 PivotField 索引。|
| [position](/cells/zh/python-net/aspose.cells.pivot/pivotfield/position) |表示 PivotFields 中的 PivotField 索引。|
| [name](/cells/zh/python-net/aspose.cells.pivot/pivotfield/name) |表示 PivotField 名称。|
| [display_name](/cells/zh/python-net/aspose.cells.pivot/pivotfield/display_name) |表示 PivotField 显示名称。|
| [is_auto_subtotals](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_auto_subtotals) |指定字段是否显示自动小计，默认为true。|
| [drag_to_column](/cells/zh/python-net/aspose.cells.pivot/pivotfield/drag_to_column) |指示指定字段是否可以拖到列位置。<br/>默认值是true。|
| [drag_to_hide](/cells/zh/python-net/aspose.cells.pivot/pivotfield/drag_to_hide) |指示指定字段是否可以拖动到隐藏位置。<br/>默认值是true。|
| [drag_to_row](/cells/zh/python-net/aspose.cells.pivot/pivotfield/drag_to_row) |指示指定字段是否可以拖动到行位置。<br/>默认值是true。|
| [drag_to_page](/cells/zh/python-net/aspose.cells.pivot/pivotfield/drag_to_page) |指示指定字段是否可以拖动到页面位置。<br/>默认值是true。|
| [drag_to_data](/cells/zh/python-net/aspose.cells.pivot/pivotfield/drag_to_data) |指示指定字段是否可以拖动到数据位置。<br/>默认值是true。|
| [is_multiple_item_selection_allowed](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_multiple_item_selection_allowed) |指示该字段是否可以有多个项目<br/>在页面字段中选择<br/>默认值为假。|
| [is_repeat_item_labels](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_repeat_item_labels) |指示该字段是否可以重复项目标签<br/>默认值为假。|
| [is_include_new_items_in_filter](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_include_new_items_in_filter) |指示该字段是否可以包含手动过滤器中的新项目<br/>默认值为假。|
| [is_insert_page_breaks_between_items](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_insert_page_breaks_between_items) |指示该字段是否可以在项目之间插入分页符<br/>在每个项目后插入分页符<br/>默认值为假。|
| [show_all_items](/cells/zh/python-net/aspose.cells.pivot/pivotfield/show_all_items) |指示是否显示数据透视表中的所有项目，<br/>即使它们不包含摘要数据。<br/>显示没有数据的项目<br/>默认值为假。|
| [non_auto_sort_default](/cells/zh/python-net/aspose.cells.pivot/pivotfield/non_auto_sort_default) |指示将应用于此数据透视字段的排序操作是自动排序操作还是简单数据排序。|
| [is_auto_sort](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_auto_sort) |指示指定的数据透视表字段是否自动排序。|
| [is_ascend_sort](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_ascend_sort) |指示指定的数据透视表字段是否按升序自动排序。|
| [auto_sort_field](/cells/zh/python-net/aspose.cells.pivot/pivotfield/auto_sort_field) |表示自动排序字段索引。<br/> -1 表示 PivotField 本身，其他表示数据字段的位置。|
| [is_auto_show](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_auto_show) |表示指定的数据透视表字段是否自动显示，只对excel 2003有效。|
| [is_ascend_show](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_ascend_show) |指示指定的数据透视表字段是否按升序自动显示。|
| [auto_show_count](/cells/zh/python-net/aspose.cells.pivot/pivotfield/auto_show_count) |表示顶部或底部项目的数量<br/>自动显示在指定的数据透视表字段中。|
| [auto_show_field](/cells/zh/python-net/aspose.cells.pivot/pivotfield/auto_show_field) |表示自动显示字段索引。-1 表示 PivotField 本身。<br/>它应该是数据字段的索引。|
| [function](/cells/zh/python-net/aspose.cells.pivot/pivotfield/function) |表示用于汇总数据透视表数据字段的函数。|
| [data_display_format](/cells/zh/python-net/aspose.cells.pivot/pivotfield/data_display_format) |表示如何显示数据字段中包含的值。|
| [base_field_index](/cells/zh/python-net/aspose.cells.pivot/pivotfield/base_field_index) |表示自定义计算的基础字段。|
| [base_item_position](/cells/zh/python-net/aspose.cells.pivot/pivotfield/base_item_position) |表示自定义计算的基本字段中的项目。<br/>仅对数据字段有效。<br/>因为PivotItemPosition.Custom只读，如果需要设置PivotItemPosition.Custom，<br/>请设置 PivotField.BaseItemIndex 属性。|
| [base_item_index](/cells/zh/python-net/aspose.cells.pivot/pivotfield/base_item_index) |表示自定义计算的基本字段中的项目。<br/>仅对数据字段有效。|
| [current_page_item](/cells/zh/python-net/aspose.cells.pivot/pivotfield/current_page_item) |表示为页面字段显示的当前页面项目（仅对页面字段有效）。|
| [number](/cells/zh/python-net/aspose.cells.pivot/pivotfield/number) |表示数字和日期的内置显示格式。|
| [insert_blank_row](/cells/zh/python-net/aspose.cells.pivot/pivotfield/insert_blank_row) |指示是否在每个项目后插入空行。|
| [show_subtotal_at_top](/cells/zh/python-net/aspose.cells.pivot/pivotfield/show_subtotal_at_top) |当 ShowInOutlineForm 为真时，则在项目列表的顶部而不是底部显示小计|
| [show_in_outline_form](/cells/zh/python-net/aspose.cells.pivot/pivotfield/show_in_outline_form) |指示是否在数据透视表视图上以大纲形式布局此字段|
| [number_format](/cells/zh/python-net/aspose.cells.pivot/pivotfield/number_format) |表示数字和日期的自定义显示格式。|
| [items](/cells/zh/python-net/aspose.cells.pivot/pivotfield/items) |获取所有基础物品；|
| [original_items](/cells/zh/python-net/aspose.cells.pivot/pivotfield/original_items) |获得原始基础物品；|
| [item_count](/cells/zh/python-net/aspose.cells.pivot/pivotfield/item_count) |获取此数据透视字段的基本项计数。|
| [show_compact](/cells/zh/python-net/aspose.cells.pivot/pivotfield/show_compact) |指示是否显示数据透视表视图中同一列中下一个字段的标签|


### 方法
|方法|描述|
| :- | :- |
| [hide_item(index, is_hidden)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/hide_item/#int-bool) |设置是否隐藏数据字段中的特定 PivotItem。|
| [hide_item(item_value, is_hidden)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/hide_item/#str-bool) |设置是否隐藏数据字段中的特定 PivotItem。|
| [get_pivot_filter_by_type(type)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/get_pivot_filter_by_type/#PivotFilterType) |按类型获取数据透视字段的数据透视过滤器|
| [get_pivot_filters()](/cells/zh/python-net/aspose.cells.pivot/pivotfield/get_pivot_filters/#) |获取数据透视字段的数据透视过滤器|
| [init_pivot_items()](/cells/zh/python-net/aspose.cells.pivot/pivotfield/init_pivot_items/#) |初始化数据透视字段的数据透视项|
| [get_calculated_field_formula()](/cells/zh/python-net/aspose.cells.pivot/pivotfield/get_calculated_field_formula/#) |获取指定计算字段的公式字符串。|
| [set_subtotals(subtotal_type, shown)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/set_subtotals/#PivotFieldSubtotalType-bool) |设置指定字段是否显示小计。|
| [get_subtotals(subtotal_type)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/get_subtotals/#PivotFieldSubtotalType) |获取指定字段是否显示小计。|
| [is_hidden_item(index)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_hidden_item/#int) |指示特定 PivotItem 是否隐藏。|
| [is_hidden_item_detail(index)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/is_hidden_item_detail/#int) |指示特定 PivotItem 是否为隐藏详细信息。|
| [hide_item_detail(index, is_hidden_detail)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/hide_item_detail/#int-bool) |设置数据透视字段中的特定 PivotItem 是否为隐藏详细信息。|
| [hide_detail(is_hidden_detail)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/hide_detail/#bool) |设置枢轴字段中的 PivotItems 是否隐藏详细信息。即折叠/展开此字段。|
| [add_calculated_item(name, formula)](/cells/zh/python-net/aspose.cells.pivot/pivotfield/add_calculated_item/#str-str) |将计算项添加到数据透视字段。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType

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
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.pivot](..)
