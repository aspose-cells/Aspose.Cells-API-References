---
title: AutoFilter类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 70
url: /zh/python-net/aspose.cells/autofilter/
is_root: false
---
##  AutoFilter类
代表指定工作表的自动筛选。



AutoFilter 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [sorter](/cells/zh/python-net/aspose.cells/autofilter/sorter) |获取数据排序器。|
| [range](/cells/zh/python-net/aspose.cells/autofilter/range) |表示指定的自动筛选器适用的范围。|
| [show_filter_button](/cells/zh/python-net/aspose.cells/autofilter/show_filter_button) |指示此列的自动筛选按钮是否可见。|
| [filter_columns](/cells/zh/python-net/aspose.cells/autofilter/filter_columns) |获取过滤列的集合。|


### 方法
|方法|描述|
| :- | :- |
| [remove_filter(field_index, criteria)](/cells/zh/python-net/aspose.cells/autofilter/remove_filter/#int-str) |删除筛选器列的筛选器。|
| [remove_filter(field_index)](/cells/zh/python-net/aspose.cells/autofilter/remove_filter/#int) |删除特定过滤器。|
| [custom(field_index, operator_type1, criteria1)](/cells/zh/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any) |使用自定义条件过滤列表。|
| [custom(field_index, operator_type1, criteria1, is_and, operator_type2, criteria2)](/cells/zh/python-net/aspose.cells/autofilter/custom/#int-FilterOperatorType-any-bool-FilterOperatorType-any) |使用自定义条件过滤列表。|
| [refresh()](/cells/zh/python-net/aspose.cells/autofilter/refresh/#) |刷新自动过滤器以隐藏或取消隐藏行。|
| [refresh(hide_rows)](/cells/zh/python-net/aspose.cells/autofilter/refresh/#bool) |获取所有隐藏行的索引。|
| [set_range(row, start_column, end_column)](/cells/zh/python-net/aspose.cells/autofilter/set_range/#int-int-int) |设置指定的自动筛选器适用的范围。|
| [get_cell_area()](/cells/zh/python-net/aspose.cells/autofilter/get_cell_area/#) |获取应用指定自动筛选器的 [CellArea](/cells/zh/python-net/aspose.cells/cellarea)。|
| [add_filter(field_index, criteria)](/cells/zh/python-net/aspose.cells/autofilter/add_filter/#int-str) |为过滤列添加过滤器。|
| [add_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/zh/python-net/aspose.cells/autofilter/add_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) |添加日期过滤器。|
| [remove_date_filter(field_index, date_time_grouping_type, year, month, day, hour, minute, second)](/cells/zh/python-net/aspose.cells/autofilter/remove_date_filter/#int-DateTimeGroupingType-int-int-int-int-int-int) |删除日期过滤器。|
| [filter(field_index, criteria)](/cells/zh/python-net/aspose.cells/autofilter/filter/#int-str) |使用指定条件过滤列表。|
| [filter_top10(field_index, is_top, is_percent, item_count)](/cells/zh/python-net/aspose.cells/autofilter/filter_top10/#int-bool-bool-int) |筛选列表中的前 10 项|
| [dynamic_filter(field_index, dynamic_filter_type)](/cells/zh/python-net/aspose.cells/autofilter/dynamic_filter/#int-DynamicFilterType) |添加动态过滤器。|
| [add_font_color_filter(field_index, color)](/cells/zh/python-net/aspose.cells/autofilter/add_font_color_filter/#int-CellsColor) |添加字体颜色过滤器。|
| [add_fill_color_filter(field_index, pattern, foreground_color, background_color)](/cells/zh/python-net/aspose.cells/autofilter/add_fill_color_filter/#int-BackgroundType-CellsColor-CellsColor) |添加填充颜色过滤器。|
| [add_icon_filter(field_index, icon_set_type, icon_id)](/cells/zh/python-net/aspose.cells/autofilter/add_icon_filter/#int-IconSetType-int) |添加图标过滤器。|
| [match_blanks(field_index)](/cells/zh/python-net/aspose.cells/autofilter/match_blanks/#int) |匹配列表中的所有空白单元格。|
| [match_non_blanks(field_index)](/cells/zh/python-net/aspose.cells/autofilter/match_non_blanks/#int) |匹配列表中所有非空白单元格。|
| [show_all()](/cells/zh/python-net/aspose.cells/autofilter/show_all/#) |取消隐藏所有行。|



### 例子

```python
from aspose.cells import Workbook

# Creating a file stream containing the Excel file to be opened
# Instantiating a Workbook object
workbook = Workbook("template.xlsx")
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating AutoFilter by giving the cells range of the heading row
worksheet.auto_filter.range = "A1:B1"
# Filtering columns with specified values
worksheet.auto_filter.filter(1, "Bananas")
# Saving the modified Excel file.
workbook.save("output.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CellArea](/cells/zh/python-net/aspose.cells/cellarea)
