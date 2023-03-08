---
title: PivotTable类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.pivot/pivottable/
is_root: false
---
##  PivotTable类
PivotTable 的摘要说明。



PivotTable 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_excel_2003_compatible](/cells/zh/python-net/aspose.cells.pivot/pivottable/is_excel_2003_compatible) |指定刷新数据透视表时数据透视表是否兼容Excel2003，<br/>如果为真，则字符串必须小于或等于 255 个字符，因此如果字符串大于 255 个字符，<br/>它将被截断。如果为 false，字符串将没有上述限制。<br/>默认值是true。|
| [refreshed_by_who](/cells/zh/python-net/aspose.cells.pivot/pivottable/refreshed_by_who) |获取上次刷新数据透视表的用户的名称|
| [refresh_date](/cells/zh/python-net/aspose.cells.pivot/pivottable/refresh_date) |获取上次刷新数据透视表的日期。|
| [pivot_table_style_name](/cells/zh/python-net/aspose.cells.pivot/pivottable/pivot_table_style_name) |获取和设置数据透视表样式名称。|
| [pivot_table_style_type](/cells/zh/python-net/aspose.cells.pivot/pivottable/pivot_table_style_type) |获取和设置内置数据透视表样式。|
| [column_fields](/cells/zh/python-net/aspose.cells.pivot/pivottable/column_fields) |返回当前显示为列字段的 PivotFields 对象。|
| [row_fields](/cells/zh/python-net/aspose.cells.pivot/pivottable/row_fields) |返回当前显示为行字段的 PivotFields 对象。|
| [page_fields](/cells/zh/python-net/aspose.cells.pivot/pivottable/page_fields) |返回当前显示为页面字段的 PivotFields 对象。|
| [data_fields](/cells/zh/python-net/aspose.cells.pivot/pivottable/data_fields) |获取表示数据透视表中所有数据字段的 PivotField 对象。<br/>只读。只有当DataPiovtFiels中有两个或多个数据字段时才会被初始化。<br/>它仅用于将 DataPivotField 添加到数据透视表的行/列区域。默认在行区域。|
| [data_field](/cells/zh/python-net/aspose.cells.pivot/pivottable/data_field) |获取表示数据透视表中所有数据字段的 PivotField 对象。<br/>只读。只有当DataPiovtFiels中有两个或多个数据字段时才会被初始化。<br/>它仅用于将 DataPivotField 添加到数据透视表的行/列区域。默认在行区域。|
| [base_fields](/cells/zh/python-net/aspose.cells.pivot/pivottable/base_fields) |返回一个 PivotFields 对象，该对象包含数据透视表中的所有字段|
| [pivot_filters](/cells/zh/python-net/aspose.cells.pivot/pivottable/pivot_filters) |返回一个 PivotFilterCollection 对象。|
| [column_range](/cells/zh/python-net/aspose.cells.pivot/pivottable/column_range) |返回表示范围的 CellArea 对象<br/>包含数据透视表中的列区域。只读。|
| [row_range](/cells/zh/python-net/aspose.cells.pivot/pivottable/row_range) |返回表示范围的 CellArea 对象<br/>包含数据透视表中的行区域。只读。|
| [data_body_range](/cells/zh/python-net/aspose.cells.pivot/pivottable/data_body_range) |返回一个 CellArea 对象，表示包含数据区域的范围<br/>在标题行和插入行之间的列表中。只读。|
| [table_range1](/cells/zh/python-net/aspose.cells.pivot/pivottable/table_range1) |返回一个 CellArea 对象，该对象表示包含整个数据透视表的区域，<br/>但不包括页面字段。只读。|
| [table_range2](/cells/zh/python-net/aspose.cells.pivot/pivottable/table_range2) |返回一个 CellArea 对象，该对象表示包含整个数据透视表的区域，<br/>包括页面字段。只读。|
| [column_grand](/cells/zh/python-net/aspose.cells.pivot/pivottable/column_grand) |指示数据透视表是否显示列的总计。|
| [is_grid_drop_zones](/cells/zh/python-net/aspose.cells.pivot/pivottable/is_grid_drop_zones) |指示数据透视表是否显示经典数据透视表布局。<br/> （允许拖动网格中的字段）|
| [row_grand](/cells/zh/python-net/aspose.cells.pivot/pivottable/row_grand) |指示数据透视表是否显示行的总计。|
| [display_null_string](/cells/zh/python-net/aspose.cells.pivot/pivottable/display_null_string) |指示数据透视表是否显示自定义字符串<br/>在包含空值的单元格中。|
| [null_string](/cells/zh/python-net/aspose.cells.pivot/pivottable/null_string) |获取显示在包含空值的单元格中的字符串<br/>当 DisplayNullString 属性为 true 时。默认值为空字符串。|
| [display_error_string](/cells/zh/python-net/aspose.cells.pivot/pivottable/display_error_string) |指示数据透视表是否在包含错误的单元格中显示自定义字符串。|
| [data_field_header_name](/cells/zh/python-net/aspose.cells.pivot/pivottable/data_field_header_name) |获取和设置数据透视表中值区域字段标题的名称。|
| [error_string](/cells/zh/python-net/aspose.cells.pivot/pivottable/error_string) |获取显示在包含错误的单元格中的字符串<br/>当 DisplayErrorString 属性为 true 时。默认值为空字符串。|
| [is_auto_format](/cells/zh/python-net/aspose.cells.pivot/pivottable/is_auto_format) |指示数据透视表是否自动设置格式。<br/>Excel 2003 的数据透视表选项中的复选框“自动格式表”<br/>数据透视表选项中的复选框“更新时自动调整列宽”：Excel 2007 的布局格式|
| [auto_format_type](/cells/zh/python-net/aspose.cells.pivot/pivottable/auto_format_type) |获取数据透视表自动格式类型。|
| [has_blank_rows](/cells/zh/python-net/aspose.cells.pivot/pivottable/has_blank_rows) |是否添加空行。<br/>此属性仅适用于需要添加空行的数据透视表自动格式类型。|
| [merge_labels](/cells/zh/python-net/aspose.cells.pivot/pivottable/merge_labels) |指示指定数据透视表的外行项、列项、小计、<br/>总计标签使用合并的单元格。|
| [preserve_formatting](/cells/zh/python-net/aspose.cells.pivot/pivottable/preserve_formatting) |指示在刷新或重新计算数据透视表时是否保留格式。|
| [show_drill](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_drill) |获取是否显示展开/折叠按钮。|
| [enable_drilldown](/cells/zh/python-net/aspose.cells.pivot/pivottable/enable_drilldown) |获取是否启用向下钻取。|
| [enable_field_dialog](/cells/zh/python-net/aspose.cells.pivot/pivottable/enable_field_dialog) |指示数据透视表字段对话框是否可用<br/>当用户双击数据透视表字段时。|
| [enable_field_list](/cells/zh/python-net/aspose.cells.pivot/pivottable/enable_field_list) |获取是否启用数据透视表的字段列表。|
| [enable_wizard](/cells/zh/python-net/aspose.cells.pivot/pivottable/enable_wizard) |指示数据透视表向导是否可用。|
| [subtotal_hidden_page_items](/cells/zh/python-net/aspose.cells.pivot/pivottable/subtotal_hidden_page_items) |指示数据透视表中是否隐藏页字段项<br/>包含在行和列小计、块总计和总计中。<br/>默认值为假。|
| [grand_total_name](/cells/zh/python-net/aspose.cells.pivot/pivottable/grand_total_name) |返回显示在总计列或行标题中的文本字符串标签。<br/>默认值为字符串“Grand Total”。|
| [manual_update](/cells/zh/python-net/aspose.cells.pivot/pivottable/manual_update) |指示是否仅在用户请求时才重新计算数据透视表。|
| [is_multiple_field_filters](/cells/zh/python-net/aspose.cells.pivot/pivottable/is_multiple_field_filters) |指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。|
| [missing_items_limit](/cells/zh/python-net/aspose.cells.pivot/pivottable/missing_items_limit) |指定一个布尔值，指示数据透视表的字段是否可以设置多个筛选器。|
| [enable_data_value_editing](/cells/zh/python-net/aspose.cells.pivot/pivottable/enable_data_value_editing) |指定一个布尔值，指示是否允许用户编辑数据透视表数据区域中的单元格。<br/>在值区域中启用单元格编辑|
| [show_data_tips](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_data_tips) |指定一个布尔值，指示是否应为数据透视表数据单元格显示工具提示。|
| [show_member_property_tips](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_member_property_tips) |指定一个布尔值，该值指示是否应从数据透视表工具提示中省略成员属性信息。|
| [show_values_row](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_values_row) |指定一个布尔值，指示是否显示值行。<br/>显示值行|
| [show_empty_col](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_empty_col) |指定一个布尔值，指示是否在表中包含空列|
| [show_empty_row](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_empty_row) |指定一个布尔值，指示是否在表中包含空行。|
| [field_list_sort_ascending](/cells/zh/python-net/aspose.cells.pivot/pivottable/field_list_sort_ascending) |指定一个布尔值，指示数据透视表中的字段是否在字段列表中按非默认顺序排序。|
| [print_drill](/cells/zh/python-net/aspose.cells.pivot/pivottable/print_drill) |指定一个布尔值，指示是否应打印钻取指示器。<br/>在数据透视表上显示时打印展开/折叠按钮。|
| [alt_text_title](/cells/zh/python-net/aspose.cells.pivot/pivottable/alt_text_title) |获取替代文本的标题|
| [alt_text_description](/cells/zh/python-net/aspose.cells.pivot/pivottable/alt_text_description) |获取替代文本的描述|
| [name](/cells/zh/python-net/aspose.cells.pivot/pivottable/name) |获取数据透视表的名称|
| [column_header_caption](/cells/zh/python-net/aspose.cells.pivot/pivottable/column_header_caption) |获取数据透视表的列标题标题。|
| [indent](/cells/zh/python-net/aspose.cells.pivot/pivottable/indent) |指定紧凑轴的缩进增量，可用于将报告布局设置为紧凑形式。|
| [row_header_caption](/cells/zh/python-net/aspose.cells.pivot/pivottable/row_header_caption) |获取数据透视表的行标题标题。|
| [show_row_header_caption](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_row_header_caption) |指示行标题标题是否显示在数据透视表中<br/>指示是否显示字段标题和过滤器下拉列表|
| [custom_list_sort](/cells/zh/python-net/aspose.cells.pivot/pivottable/custom_list_sort) |表示排序数据时是否考虑内置自定义列表|
| [pivot_format_conditions](/cells/zh/python-net/aspose.cells.pivot/pivottable/pivot_format_conditions) |获取数据透视表的格式条件。|
| [page_field_order](/cells/zh/python-net/aspose.cells.pivot/pivottable/page_field_order) |获取页面字段添加到数据透视表布局的顺序。|
| [page_field_wrap_count](/cells/zh/python-net/aspose.cells.pivot/pivottable/page_field_wrap_count) |获取数据透视表中每列或每行的页字段数。|
| [tag](/cells/zh/python-net/aspose.cells.pivot/pivottable/tag) |获取与数据透视表一起保存的字符串。|
| [save_data](/cells/zh/python-net/aspose.cells.pivot/pivottable/save_data) |指示数据透视表的数据是否与工作簿一起保存。|
| [refresh_data_on_opening_file](/cells/zh/python-net/aspose.cells.pivot/pivottable/refresh_data_on_opening_file) |指示是否在打开文件时刷新数据。|
| [refresh_data_flag](/cells/zh/python-net/aspose.cells.pivot/pivottable/refresh_data_flag) |指示是否刷新数据。|
| [external_connection_data_source](/cells/zh/python-net/aspose.cells.pivot/pivottable/external_connection_data_source) |获取外部连接数据源。|
| [data_source](/cells/zh/python-net/aspose.cells.pivot/pivottable/data_source) |获取和设置数据透视表的数据源。|
| [item_print_titles](/cells/zh/python-net/aspose.cells.pivot/pivottable/item_print_titles) |指定是否在行轴上透视项目标题的位<br/>在表格形式的数据透视字段的每个打印页面上重复。|
| [print_titles](/cells/zh/python-net/aspose.cells.pivot/pivottable/print_titles) |指示工作表的打印标题是否设置为基于<br/>在数据透视表上。默认值为假。|
| [display_immediate_items](/cells/zh/python-net/aspose.cells.pivot/pivottable/display_immediate_items) |指示行和列区域中的项目是否可见<br/>当数据透视表的数据区域为空时。默认值是true。|
| [is_selected](/cells/zh/python-net/aspose.cells.pivot/pivottable/is_selected) |指示是否选择了数据透视表。|
| [show_pivot_style_row_header](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_header) |指示数据透视表中的行标题是否应应用样式。|
| [show_pivot_style_column_header](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_header) |指示数据透视表中的列标题是否应应用样式。|
| [show_pivot_style_row_stripes](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_pivot_style_row_stripes) |指示是否应用行条纹格式。|
| [show_pivot_style_column_stripes](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_pivot_style_column_stripes) |指示是否应用列条纹格式。|
| [show_pivot_style_last_column](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_pivot_style_last_column) |指示是否应用列条纹格式。|


### 方法
|方法|描述|
| :- | :- |
| [remove_field(field_type, field_name)](/cells/zh/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-str) |从特定字段区域中删除字段|
| [remove_field(field_type, base_field_index)](/cells/zh/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-int) |从特定字段区域中删除字段|
| [remove_field(field_type, pivot_field)](/cells/zh/python-net/aspose.cells.pivot/pivottable/remove_field/#PivotFieldType-PivotField) |从特定字段区域中删除字段|
| [add_field_to_area(field_type, field_name)](/cells/zh/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-str) |将字段添加到特定区域。|
| [add_field_to_area(field_type, base_field_index)](/cells/zh/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-int) |将字段添加到特定区域。|
| [add_field_to_area(field_type, pivot_field)](/cells/zh/python-net/aspose.cells.pivot/pivottable/add_field_to_area/#PivotFieldType-PivotField) |将字段添加到特定区域。|
| [add_calculated_field(name, formula, drag_to_data_area)](/cells/zh/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str-bool) |将计算字段添加到数据透视字段。|
| [add_calculated_field(name, formula)](/cells/zh/python-net/aspose.cells.pivot/pivottable/add_calculated_field/#str-str) |将计算字段添加到数据透视字段并将其拖动到数据区域。|
| [move(row, column)](/cells/zh/python-net/aspose.cells.pivot/pivottable/move/#int-int) |将数据透视表移动到工作表中的不同位置。|
| [move(dest_cell_name)](/cells/zh/python-net/aspose.cells.pivot/pivottable/move/#str) |将数据透视表移动到工作表中的不同位置。|
| [set_auto_group_field(base_field_index)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#int) |通过数据透视表设置自动字段组。|
| [set_auto_group_field(pivot_field)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_auto_group_field/#PivotField) |通过数据透视表设置自动字段组。|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-float-float-list-float) |通过数据透视表设置手动字段组。|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-float-float-list-float) |通过数据透视表设置手动字段组。|
| [set_manual_group_field(base_field_index, start_val, end_val, group_by_list, interval_num)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#int-DateTime-DateTime-list-int) |通过数据透视表设置手动字段组。|
| [set_manual_group_field(pivot_field, start_val, end_val, group_by_list, interval_num)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_manual_group_field/#PivotField-DateTime-DateTime-list-int) |通过数据透视表设置手动字段组。|
| [set_ungroup(base_field_index)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_ungroup/#int) |按数据透视表设置取消分组|
| [set_ungroup(pivot_field)](/cells/zh/python-net/aspose.cells.pivot/pivottable/set_ungroup/#PivotField) |按数据透视表设置取消分组|
| [copy_style(pivot_table)](/cells/zh/python-net/aspose.cells.pivot/pivottable/copy_style/#PivotTable) |从另一个数据透视表复制命名样式。|
| [show_report_filter_page(page_field)](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_report_filter_page/#PivotField) |根据 PivotField 显示所有报表筛选页面，PivotField 必须位于 PageFields 中。|
| [show_report_filter_page_by_name(field_name)](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_name/#str) |根据 PivotField 的名称显示所有报表筛选页面，PivotField 必须位于 PageFields 中。|
| [show_report_filter_page_by_index(pos_index)](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_report_filter_page_by_index/#int) |根据PageFields中的位置索引显示所有报表过滤页面|
| [fields(field_type)](/cells/zh/python-net/aspose.cells.pivot/pivottable/fields/#PivotFieldType) |按字段类型获取特定字段。|
| [change_data_source(source)](/cells/zh/python-net/aspose.cells.pivot/pivottable/change_data_source/#list) |设置数据透视表的源数据。<br/>工作表 1!$A$1:$C$3|
| [get_source()](/cells/zh/python-net/aspose.cells.pivot/pivottable/get_source/#) |获取数据透视表的源数据。|
| [refresh_data()](/cells/zh/python-net/aspose.cells.pivot/pivottable/refresh_data/#) |从数据源刷新数据透视表的数据和设置。|
| [calculate_data()](/cells/zh/python-net/aspose.cells.pivot/pivottable/calculate_data/#) |将数据透视表的数据计算到单元格。|
| [clear_data()](/cells/zh/python-net/aspose.cells.pivot/pivottable/clear_data/#) |清除数据透视表的数据和格式|
| [calculate_range()](/cells/zh/python-net/aspose.cells.pivot/pivottable/calculate_range/#) |计算数据透视表的范围。|
| [format_all(style)](/cells/zh/python-net/aspose.cells.pivot/pivottable/format_all/#Style) |格式化数据透视表区域中的所有单元格|
| [format_row(row, style)](/cells/zh/python-net/aspose.cells.pivot/pivottable/format_row/#int-Style) |格式化数据透视表区域中的行数据|
| [format(row, column, style)](/cells/zh/python-net/aspose.cells.pivot/pivottable/format/#int-int-Style) |格式化数据透视区域中的单元格|
| [get_horizontal_breaks()](/cells/zh/python-net/aspose.cells.pivot/pivottable/get_horizontal_breaks/#) |获取水平分页符的数据透视表行索引列表|
| [show_in_compact_form()](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_in_compact_form/#) |以紧凑的形式布置数据透视表。|
| [show_in_outline_form()](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_in_outline_form/#) |以大纲形式布置数据透视表。|
| [show_in_tabular_form()](/cells/zh/python-net/aspose.cells.pivot/pivottable/show_in_tabular_form/#) |以表格形式布置数据透视表。|
| [get_cell_by_display_name(display_name)](/cells/zh/python-net/aspose.cells.pivot/pivottable/get_cell_by_display_name/#str) |通过 PivotField 的 DisplayName 获取 Cell 对象|
| [get_children()](/cells/zh/python-net/aspose.cells.pivot/pivottable/get_children/#) |获取使用此数据透视表数据作为数据源的子数据透视表。|



### 例子

```python
from aspose.cells import FormatConditionType, OperatorType, Workbook
from aspose.cells.pivot import PivotFieldType, PivotFilterType, PivotTableStyleType
from aspose.pydrawing import Color

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
# Add PivotFilter
index = pivot.pivot_filters.add(0, PivotFilterType.COUNT)
filter = pivot.pivot_filters[index]
filter.auto_filter.filter_top10(0, False, False, 2)
# Add PivotFormatCondition
formatIndex = pivot.pivot_format_conditions.add()
pfc = pivot.pivot_format_conditions[formatIndex]
fcc = pfc.format_conditions
fcc.add_area(pivot.data_body_range)
idx = fcc.add_condition(FormatConditionType.CELL_VALUE)
fc = fcc[idx]
fc.formula1 = "100"
fc.operator = OperatorType.GREATER_OR_EQUAL
fc.style.background_color = Color.red
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.pivot](..)
