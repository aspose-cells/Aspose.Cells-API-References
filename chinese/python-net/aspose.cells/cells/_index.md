---
title: Cells类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells/cells/
is_root: false
---
## Cells类
封装单元格相关对象的集合，例如 [Cell](/cells/zh/python-net/aspose.cells/cell)、[Row](/cells/zh/python-net/aspose.cells/row) 等。



Cells 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [ods_cell_fields](/cells/zh/python-net/aspose.cells/cells/ods_cell_fields) |获取ods的字段列表。|
| [count](/cells/zh/python-net/aspose.cells/cells/count) |获取实例化的 Cell 对象的总数。|
| [count_large](/cells/zh/python-net/aspose.cells/cells/count_large) |获取实例化的 Cell 对象的总数。|
| [rows](/cells/zh/python-net/aspose.cells/cells/rows) |获取表示此工作表中各行的 [Row](/cells/zh/python-net/aspose.cells/row) 对象的集合。|
| [merged_cells](/cells/zh/python-net/aspose.cells/cells/merged_cells) |获取合并单元格的集合。|
| [multi_thread_reading](/cells/zh/python-net/aspose.cells/cells/multi_thread_reading) |获取或设置单元格数据模型是否应支持多线程读取。<br/>此属性的默认值为 false。|
| [memory_setting](/cells/zh/python-net/aspose.cells/cells/memory_setting) |获取或设置此单元格的内存使用选项。|
| [style](/cells/zh/python-net/aspose.cells/cells/style) |获取和设置默认样式。|
| [standard_width_inch](/cells/zh/python-net/aspose.cells/cells/standard_width_inch) |获取或设置工作表中的默认列宽，以英寸为单位。|
| [standard_width_pixels](/cells/zh/python-net/aspose.cells/cells/standard_width_pixels) |获取或设置工作表中的默认列宽，以像素为单位。|
| [standard_width](/cells/zh/python-net/aspose.cells/cells/standard_width) |获取或设置工作表中的默认列宽，以字符为单位。|
| [standard_height](/cells/zh/python-net/aspose.cells/cells/standard_height) |获取或设置此工作表中的默认行高，以磅为单位。|
| [standard_height_pixels](/cells/zh/python-net/aspose.cells/cells/standard_height_pixels) |获取或设置此工作表中的默认行高，以像素为单位。|
| [standard_height_inch](/cells/zh/python-net/aspose.cells/cells/standard_height_inch) |获取或设置此工作表中的默认行高，以英寸为单位。|
| [preserve_string](/cells/zh/python-net/aspose.cells/cells/preserve_string) |获取或设置一个值，该值指示是否所有工作表值都保留为字符串。<br/>默认为假。|
| [min_row](/cells/zh/python-net/aspose.cells/cells/min_row) |包含数据或样式的单元格的最小行索引。|
| [max_row](/cells/zh/python-net/aspose.cells/cells/max_row) |包含数据或样式的单元格的最大行索引。|
| [min_column](/cells/zh/python-net/aspose.cells/cells/min_column) |已在集合中实例化的那些单元格的最小列索引（不包括列<br/>其中为整列定义了样式，但其中没有实例化单元格）。|
| [max_column](/cells/zh/python-net/aspose.cells/cells/max_column) |已在集合中实例化的那些单元格的最小列索引（不包括列<br/>其中为整列定义了样式，但其中没有实例化单元格）。|
| [min_data_row](/cells/zh/python-net/aspose.cells/cells/min_data_row) |包含数据的单元格的最小行索引。|
| [max_data_row](/cells/zh/python-net/aspose.cells/cells/max_data_row) |包含数据的单元格的最大行索引。|
| [min_data_column](/cells/zh/python-net/aspose.cells/cells/min_data_column) |包含数据的单元格的最小列索引。|
| [max_data_column](/cells/zh/python-net/aspose.cells/cells/max_data_column) |包含数据的单元格的最大列索引。|
| [is_default_row_height_matched](/cells/zh/python-net/aspose.cells/cells/is_default_row_height_matched) |指示行高和默认字体高度匹配|
| [is_default_row_hidden](/cells/zh/python-net/aspose.cells/cells/is_default_row_hidden) |指示该行是否默认隐藏。|
| [columns](/cells/zh/python-net/aspose.cells/cells/columns) |获取表示此工作表中各个列的 [Column](/cells/zh/python-net/aspose.cells/column) 对象的集合。|
| [ranges](/cells/zh/python-net/aspose.cells/cells/ranges) |获取在运行时创建的 [Range](/cells/zh/python-net/aspose.cells/range) 对象的集合。|
| [last_cell](/cells/zh/python-net/aspose.cells/cells/last_cell) |获取此工作表中的最后一个单元格。|
| [max_display_range](/cells/zh/python-net/aspose.cells/cells/max_display_range) |获取包括数据、合并的单元格和形状的最大范围。|
| [first_cell](/cells/zh/python-net/aspose.cells/cells/first_cell) |获取此工作表中的第一个单元格。|



获取工作表中的 [Cell](/cells/zh/python-net/aspose.cells/cell) 项
### 索引器
|名称|描述|
| :- | :- |
| [index] |元素的从零开始的索引。|


### 方法
|方法|描述|
| :- | :- |
| [create_range(upper_left_cell, lower_right_cell)](/cells/zh/python-net/aspose.cells/cells/create_range/#str-str) |从一系列单元格创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。|
| [create_range(first_row, first_column, total_rows, total_columns)](/cells/zh/python-net/aspose.cells/cells/create_range/#int-int-int-int) |从一系列单元格创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。|
| [create_range(address)](/cells/zh/python-net/aspose.cells/cells/create_range/#str) |从范围地址创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。|
| [create_range(first_index, number, is_vertical)](/cells/zh/python-net/aspose.cells/cells/create_range/#int-int-bool) |从单元格行或单元格列创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。|
| [get(row, column)](/cells/zh/python-net/aspose.cells/cells/get/#int-int) |添加 API for Python 通过 .Net.since this[int row, int column] 不受支持|
| [get(cell_name)](/cells/zh/python-net/aspose.cells/cells/get/#str) |添加 API for Python 通过 .Net.since this[string cellName] 不受支持|
| [import_object_array(obj_array, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool) |将数据数组导入工作表。|
| [import_object_array(obj_array, first_row, first_column, is_vertical, skip)](/cells/zh/python-net/aspose.cells/cells/import_object_array/#list-int-int-bool-int) |将数据数组导入工作表。|
| [import_array(string_array, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_array/#list-int-int-bool) |将字符串数组导入工作表。|
| [import_array(int_array, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_array/#list-int-int-bool) |将整数数组导入工作表。|
| [import_array(double_array, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_array/#list-int-int-bool) |将双精度数组导入工作表。|
| [import_csv(file_name, splitter, convert_numeric_data, first_row, first_column)](/cells/zh/python-net/aspose.cells/cells/import_csv/#str-str-bool-int-int) |将 CSV 文件导入单元格。|
| [import_csv(stream, splitter, convert_numeric_data, first_row, first_column)](/cells/zh/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-str-bool-int-int) |将 CSV 文件导入单元格。|
| [import_csv(file_name, options, first_row, first_column)](/cells/zh/python-net/aspose.cells/cells/import_csv/#str-TxtLoadOptions-int-int) |将 CSV 文件导入单元格。|
| [import_csv(stream, options, first_row, first_column)](/cells/zh/python-net/aspose.cells/cells/import_csv/#io.RawIOBase-TxtLoadOptions-int-int) |将 CSV 文件导入单元格。|
| [merge(first_row, first_column, total_rows, total_columns)](/cells/zh/python-net/aspose.cells/cells/merge/#int-int-int-int) |将指定范围的单元格合并为一个单元格。|
| [merge(first_row, first_column, total_rows, total_columns, merge_conflict)](/cells/zh/python-net/aspose.cells/cells/merge/#int-int-int-int-bool) |将指定范围的单元格合并为一个单元格。|
| [merge(first_row, first_column, total_rows, total_columns, check_conflict, merge_conflict)](/cells/zh/python-net/aspose.cells/cells/merge/#int-int-int-int-bool-bool) |将指定范围的单元格合并为一个单元格。|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number, paste_options)](/cells/zh/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-PasteOptions) |复制整个列的数据和格式。|
| [copy_columns(source_cells0, source_column_index, destination_column_index, column_number)](/cells/zh/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int) |复制整个列的数据和格式。|
| [copy_columns(source_cells, source_column_index, source_total_columns, destination_column_index, destination_total_columns)](/cells/zh/python-net/aspose.cells/cells/copy_columns/#Cells-int-int-int-int) |复制整个列的数据和格式。|
| [copy_rows(source_cells, source_row_index, destination_row_index, row_number)](/cells/zh/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int) |复制一些整行的数据和格式。|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options)](/cells/zh/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions) |复制一些整行的数据和格式。|
| [copy_rows(source_cells0, source_row_index, destination_row_index, row_number, copy_options, paste_options)](/cells/zh/python-net/aspose.cells/cells/copy_rows/#Cells-int-int-int-CopyOptions-PasteOptions) |复制一些整行的数据和格式。|
| [group_columns(first_index, last_index)](/cells/zh/python-net/aspose.cells/cells/group_columns/#int-int) |组列。|
| [group_columns(first_index, last_index, is_hidden)](/cells/zh/python-net/aspose.cells/cells/group_columns/#int-int-bool) |组列。|
| [ungroup_rows(first_index, last_index, is_all)](/cells/zh/python-net/aspose.cells/cells/ungroup_rows/#int-int-bool) |取消分组行。|
| [ungroup_rows(first_index, last_index)](/cells/zh/python-net/aspose.cells/cells/ungroup_rows/#int-int) |取消分组行。|
| [group_rows(first_index, last_index, is_hidden)](/cells/zh/python-net/aspose.cells/cells/group_rows/#int-int-bool) |分组行。|
| [group_rows(first_index, last_index)](/cells/zh/python-net/aspose.cells/cells/group_rows/#int-int) |分组行。|
| [delete_column(column_index, update_reference)](/cells/zh/python-net/aspose.cells/cells/delete_column/#int-bool) |删除列。|
| [delete_column(column_index)](/cells/zh/python-net/aspose.cells/cells/delete_column/#int) |删除列。|
| [delete_rows(row_index, total_rows)](/cells/zh/python-net/aspose.cells/cells/delete_rows/#int-int) |删除多行。|
| [delete_rows(row_index, total_rows, update_reference)](/cells/zh/python-net/aspose.cells/cells/delete_rows/#int-int-bool) |删除工作表中的多行。|
| [delete_blank_columns()](/cells/zh/python-net/aspose.cells/cells/delete_blank_columns/#) |删除所有不包含任何数据的空白列。|
| [delete_blank_columns(options)](/cells/zh/python-net/aspose.cells/cells/delete_blank_columns/#DeleteOptions) |删除所有不包含任何数据的空白列。|
| [delete_blank_rows()](/cells/zh/python-net/aspose.cells/cells/delete_blank_rows/#) |删除所有不包含任何数据的空白行。|
| [delete_blank_rows(options)](/cells/zh/python-net/aspose.cells/cells/delete_blank_rows/#DeleteOptions) |删除所有不包含任何数据的空白行。|
| [insert_columns(column_index, total_columns)](/cells/zh/python-net/aspose.cells/cells/insert_columns/#int-int) |在工作表中插入一些列。|
| [insert_columns(column_index, total_columns, update_reference)](/cells/zh/python-net/aspose.cells/cells/insert_columns/#int-int-bool) |在工作表中插入一些列。|
| [insert_column(column_index, update_reference)](/cells/zh/python-net/aspose.cells/cells/insert_column/#int-bool) |在工作表中插入一个新列。|
| [insert_column(column_index)](/cells/zh/python-net/aspose.cells/cells/insert_column/#int) |在工作表中插入一个新列。|
| [insert_rows(row_index, total_rows, update_reference)](/cells/zh/python-net/aspose.cells/cells/insert_rows/#int-int-bool) |在工作表中插入多行。|
| [insert_rows(row_index, total_rows, options)](/cells/zh/python-net/aspose.cells/cells/insert_rows/#int-int-InsertOptions) |在工作表中插入多行。|
| [insert_rows(row_index, total_rows)](/cells/zh/python-net/aspose.cells/cells/insert_rows/#int-int) |在工作表中插入多行。|
| [clear_range(range)](/cells/zh/python-net/aspose.cells/cells/clear_range/#CellArea) |清除范围的内容和格式。|
| [clear_range(start_row, start_column, end_row, end_column)](/cells/zh/python-net/aspose.cells/cells/clear_range/#int-int-int-int) |清除范围的内容和格式。|
| [clear_contents(range)](/cells/zh/python-net/aspose.cells/cells/clear_contents/#CellArea) |清除范围的内容。|
| [clear_contents(start_row, start_column, end_row, end_column)](/cells/zh/python-net/aspose.cells/cells/clear_contents/#int-int-int-int) |清除范围的内容。|
| [clear_formats(range)](/cells/zh/python-net/aspose.cells/cells/clear_formats/#CellArea) |清除范围的格式。|
| [clear_formats(start_row, start_column, end_row, end_column)](/cells/zh/python-net/aspose.cells/cells/clear_formats/#int-int-int-int) |清除范围的格式。|
| [find(what, previous_cell)](/cells/zh/python-net/aspose.cells/cells/find/#any-Cell) |查找包含输入对象的单元格。|
| [find(what, previous_cell, find_options)](/cells/zh/python-net/aspose.cells/cells/find/#any-Cell-FindOptions) |查找包含输入对象的单元格。|
| [end_cell_in_row(row_index)](/cells/zh/python-net/aspose.cells/cells/end_cell_in_row/#int) |获取此行中的最后一个单元格。|
| [end_cell_in_row(start_row, end_row, start_column, end_column)](/cells/zh/python-net/aspose.cells/cells/end_cell_in_row/#int-int-int-int) |获取此范围内具有最大行索引的最后一个单元格。|
| [end_cell_in_column(column_index)](/cells/zh/python-net/aspose.cells/cells/end_cell_in_column/#int) |获取此列中的最后一个单元格。|
| [end_cell_in_column(start_row, end_row, start_column, end_column)](/cells/zh/python-net/aspose.cells/cells/end_cell_in_column/#int-int-int-int) |获取此范围内具有最大列索引的最后一个单元格。|
| [insert_range(area, shift_number, shift_type, update_reference)](/cells/zh/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType-bool) |根据移位选项插入一系列单元格和移位单元格。|
| [insert_range(area, shift_type)](/cells/zh/python-net/aspose.cells/cells/insert_range/#CellArea-ShiftType) |根据移位选项插入一系列单元格和移位单元格。|
| [insert_range(area, shift_number, shift_type)](/cells/zh/python-net/aspose.cells/cells/insert_range/#CellArea-int-ShiftType) |根据移位选项插入一系列单元格和移位单元格。|
| [import_custom_objects(list, property_names, is_property_name_shown, first_row, first_column, row_number, insert_rows, date_format_string, convert_string_to_number)](/cells/zh/python-net/aspose.cells/cells/import_custom_objects/#list-list-bool-int-int-int-bool-str-bool) |导入自定义对象。|
| [import_custom_objects(list, first_row, first_column, options)](/cells/zh/python-net/aspose.cells/cells/import_custom_objects/#list-int-int-ImportTableOptions) |导入自定义对象。|
| [subtotal(ca, group_by, function, total_list)](/cells/zh/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list) |创建范围的小计。|
| [subtotal(ca, group_by, function, total_list, replace, page_breaks, summary_below_data)](/cells/zh/python-net/aspose.cells/cells/subtotal/#CellArea-int-ConsolidationFunction-list-bool-bool-bool) |创建范围的小计。|
| [remove_duplicates()](/cells/zh/python-net/aspose.cells/cells/remove_duplicates/#) |删除工作表中的重复行。|
| [remove_duplicates(start_row, start_column, end_row, end_column)](/cells/zh/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int) |删除范围内的重复值。|
| [remove_duplicates(start_row, start_column, end_row, end_column, has_headers, column_offsets)](/cells/zh/python-net/aspose.cells/cells/remove_duplicates/#int-int-int-int-bool-list) |删除范围的重复数据。|
| [get_row_enumerator()](/cells/zh/python-net/aspose.cells/cells/get_row_enumerator/#) |获取行枚举器。|
| [get_cell(row, column)](/cells/zh/python-net/aspose.cells/cells/get_cell/#int-int) |获取指定单元格行索引和列索引处的 [Cell](/cells/zh/python-net/aspose.cells/cell) 元素或 null。|
| [get_row(row)](/cells/zh/python-net/aspose.cells/cells/get_row/#int) |获取指定单元格行索引处的 [Row](/cells/zh/python-net/aspose.cells/row) 元素。|
| [check_cell(row, column)](/cells/zh/python-net/aspose.cells/cells/check_cell/#int-int) |获取指定单元格行索引和列索引处的 [Cell](/cells/zh/python-net/aspose.cells/cell) 元素或 null。|
| [check_row(row)](/cells/zh/python-net/aspose.cells/cells/check_row/#int) |获取 [Row](/cells/zh/python-net/aspose.cells/row) 元素或指定单元格行索引处。|
| [check_column(column_index)](/cells/zh/python-net/aspose.cells/cells/check_column/#int) |获取指定列索引处的 [Column](/cells/zh/python-net/aspose.cells/column) 元素或 null。|
| [is_row_hidden(row_index)](/cells/zh/python-net/aspose.cells/cells/is_row_hidden/#int) |检查给定索引处的行是否隐藏。|
| [is_column_hidden(column_index)](/cells/zh/python-net/aspose.cells/cells/is_column_hidden/#int) |检查给定索引处的列是否隐藏。|
| [add_range(range_object)](/cells/zh/python-net/aspose.cells/cells/add_range/#Range) |向单元格添加范围对象引用|
| [clear()](/cells/zh/python-net/aspose.cells/cells/clear/#) |清除所有单元格和行对象。|
| [import_data(table, first_row, first_column, options)](/cells/zh/python-net/aspose.cells/cells/import_data/#ICellsDataTable-int-int-ImportTableOptions) |从自定义数据表导入数据。|
| [import_array_list(array_list, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_array_list/#list-int-int-bool) |将数据数组列表导入工作表。|
| [import_formula_array(string_array, first_row, first_column, is_vertical)](/cells/zh/python-net/aspose.cells/cells/import_formula_array/#list-int-int-bool) |将公式数组导入工作表。|
| [text_to_columns(row, column, total_rows, options)](/cells/zh/python-net/aspose.cells/cells/text_to_columns/#int-int-int-TxtLoadOptions) |将列中的文本拆分为多列。|
| [un_merge(first_row, first_column, total_rows, total_columns)](/cells/zh/python-net/aspose.cells/cells/un_merge/#int-int-int-int) |取消合并指定范围的合并单元格。|
| [clear_merged_cells()](/cells/zh/python-net/aspose.cells/cells/clear_merged_cells/#) |清除所有合并范围。|
| [hide_row(row)](/cells/zh/python-net/aspose.cells/cells/hide_row/#int) |隐藏一行。|
| [unhide_row(row, height)](/cells/zh/python-net/aspose.cells/cells/unhide_row/#int-float) |取消隐藏一行。|
| [hide_rows(row, total_rows)](/cells/zh/python-net/aspose.cells/cells/hide_rows/#int-int) |隐藏多行。|
| [unhide_rows(row, total_rows, height)](/cells/zh/python-net/aspose.cells/cells/unhide_rows/#int-int-float) |取消隐藏隐藏的行。|
| [set_row_height_pixel(row, pixels)](/cells/zh/python-net/aspose.cells/cells/set_row_height_pixel/#int-int) |以像素为单位设置行高。|
| [set_row_height_inch(row, inches)](/cells/zh/python-net/aspose.cells/cells/set_row_height_inch/#int-float) |以英寸为单位设置行高。|
| [set_row_height(row, height)](/cells/zh/python-net/aspose.cells/cells/set_row_height/#int-float) |设置指定行的高度。|
| [get_row_original_height_point(row)](/cells/zh/python-net/aspose.cells/cells/get_row_original_height_point/#int) |如果行被隐藏，则以点为单位获取原始行的高度|
| [hide_column(column)](/cells/zh/python-net/aspose.cells/cells/hide_column/#int) |隐藏一列。|
| [unhide_column(column, width)](/cells/zh/python-net/aspose.cells/cells/unhide_column/#int-float) |取消隐藏列|
| [hide_columns(column, total_columns)](/cells/zh/python-net/aspose.cells/cells/hide_columns/#int-int) |隐藏多列。|
| [unhide_columns(column, total_columns, width)](/cells/zh/python-net/aspose.cells/cells/unhide_columns/#int-int-float) |取消隐藏多列。|
| [get_row_height(row)](/cells/zh/python-net/aspose.cells/cells/get_row_height/#int) |获取指定行的高度。|
| [get_view_row_height(row)](/cells/zh/python-net/aspose.cells/cells/get_view_row_height/#int) |获取指定行的高度。|
| [get_row_height_pixel(row)](/cells/zh/python-net/aspose.cells/cells/get_row_height_pixel/#int) |以像素为单位获取指定行的高度。|
| [get_row_height_inch(row)](/cells/zh/python-net/aspose.cells/cells/get_row_height_inch/#int) |以英寸为单位获取指定行的高度。|
| [get_view_row_height_inch(row)](/cells/zh/python-net/aspose.cells/cells/get_view_row_height_inch/#int) |以英寸为单位获取指定行的高度。|
| [set_column_width_pixel(column, pixels)](/cells/zh/python-net/aspose.cells/cells/set_column_width_pixel/#int-int) |在普通视图中以像素为单位设置列宽。|
| [set_column_width_inch(column, inches)](/cells/zh/python-net/aspose.cells/cells/set_column_width_inch/#int-float) |在普通视图中以英寸为单位设置列宽。|
| [set_column_width(column, width)](/cells/zh/python-net/aspose.cells/cells/set_column_width/#int-float) |在普通视图中设置指定列的宽度。|
| [get_column_width_pixel(column)](/cells/zh/python-net/aspose.cells/cells/get_column_width_pixel/#int) |获取指定列在普通视图中的宽度，单位为像素。|
| [get_column_width_inch(column)](/cells/zh/python-net/aspose.cells/cells/get_column_width_inch/#int) |获取指定列在普通视图中的宽度，单位为英寸。|
| [get_column_width(column)](/cells/zh/python-net/aspose.cells/cells/get_column_width/#int) |获取普通视图下指定列的宽度|
| [get_view_column_width_pixel(column)](/cells/zh/python-net/aspose.cells/cells/get_view_column_width_pixel/#int) |获取不同视图类型的宽度。|
| [set_view_column_width_pixel(column, pixels)](/cells/zh/python-net/aspose.cells/cells/set_view_column_width_pixel/#int-int) |设置不同视图中列的宽度。|
| [get_last_data_row(column)](/cells/zh/python-net/aspose.cells/cells/get_last_data_row/#int) |获取包含指定列中数据的单元格的最后一行索引。|
| [apply_column_style(column, style, flag)](/cells/zh/python-net/aspose.cells/cells/apply_column_style/#int-Style-StyleFlag) |为整列应用格式。|
| [apply_row_style(row, style, flag)](/cells/zh/python-net/aspose.cells/cells/apply_row_style/#int-Style-StyleFlag) |为整行应用格式。|
| [apply_style(style, flag)](/cells/zh/python-net/aspose.cells/cells/apply_style/#Style-StyleFlag) |为整个工作表应用格式。|
| [copy_column(source_cells, source_column_index, destination_column_index)](/cells/zh/python-net/aspose.cells/cells/copy_column/#Cells-int-int) |复制整个列的数据和格式。|
| [copy_row(source_cells, source_row_index, destination_row_index)](/cells/zh/python-net/aspose.cells/cells/copy_row/#Cells-int-int) |复制整行的数据和格式。|
| [get_grouped_row_outline_level(row_index)](/cells/zh/python-net/aspose.cells/cells/get_grouped_row_outline_level/#int) |获取行的大纲级别（从零开始）。|
| [get_grouped_column_outline_level(column_index)](/cells/zh/python-net/aspose.cells/cells/get_grouped_column_outline_level/#int) |获取列的大纲级别（从零开始）。|
| [get_max_grouped_column_outline_level()](/cells/zh/python-net/aspose.cells/cells/get_max_grouped_column_outline_level/#) |获取最大分组列大纲级别（从零开始）。|
| [get_max_grouped_row_outline_level()](/cells/zh/python-net/aspose.cells/cells/get_max_grouped_row_outline_level/#) |获取最大分组行大纲级别（从零开始）。|
| [show_group_detail(is_vertical, index)](/cells/zh/python-net/aspose.cells/cells/show_group_detail/#bool-int) |展开分组的行/列。|
| [hide_group_detail(is_vertical, index)](/cells/zh/python-net/aspose.cells/cells/hide_group_detail/#bool-int) |折叠分组的行/列。|
| [ungroup_columns(first_index, last_index)](/cells/zh/python-net/aspose.cells/cells/ungroup_columns/#int-int) |取消分组列。|
| [delete_columns(column_index, total_columns, update_reference)](/cells/zh/python-net/aspose.cells/cells/delete_columns/#int-int-bool) |删除多个列。|
| [is_deleting_range_enabled(start_row, start_column, total_rows, total_columns)](/cells/zh/python-net/aspose.cells/cells/is_deleting_range_enabled/#int-int-int-int) |检查是否可以删除范围。|
| [delete_row(row_index)](/cells/zh/python-net/aspose.cells/cells/delete_row/#int) |删除一行。|
| [is_blank_column(column_index)](/cells/zh/python-net/aspose.cells/cells/is_blank_column/#int) |检查给定列是否为空（不包含任何数据）。|
| [insert_row(row_index)](/cells/zh/python-net/aspose.cells/cells/insert_row/#int) |在工作表中插入一个新行。|
| [link_to_xml_map(map_name, row, column, path)](/cells/zh/python-net/aspose.cells/cells/link_to_xml_map/#str-int-int-str) |链接到 xml 映射。|
| [find_formula(formula, previous_cell)](/cells/zh/python-net/aspose.cells/cells/find_formula/#str-Cell) |查找包含输入字符串的单元格。|
| [find_formula_contains(formula, previous_cell)](/cells/zh/python-net/aspose.cells/cells/find_formula_contains/#str-Cell) |查找包含输入字符串的公式的单元格。|
| [move_range(source_area, dest_row, dest_column)](/cells/zh/python-net/aspose.cells/cells/move_range/#CellArea-int-int) |移动范围。|
| [insert_cut_cells(cut_range, row, column, shift_type)](/cells/zh/python-net/aspose.cells/cells/insert_cut_cells/#Range-int-int-ShiftType) |插入切割范围。|
| [delete_range(start_row, start_column, end_row, end_column, shift_type)](/cells/zh/python-net/aspose.cells/cells/delete_range/#int-int-int-int-ShiftType) |根据移位选项删除一系列单元格和移位单元格。|
| [retrieve_subtotal_setting(ca)](/cells/zh/python-net/aspose.cells/cells/retrieve_subtotal_setting/#CellArea) |检索范围的小计设置。|
| [remove_formulas()](/cells/zh/python-net/aspose.cells/cells/remove_formulas/#) |删除所有公式并替换为公式的值。|
| [convert_string_to_numeric_value()](/cells/zh/python-net/aspose.cells/cells/convert_string_to_numeric_value/#) |如果可能，将单元格中的字符串数据转换为数值。|
| [get_dependents(is_all, row, column)](/cells/zh/python-net/aspose.cells/cells/get_dependents/#bool-int-int) |获取引用特定单元格的所有单元格。|
| [get_dependents_in_calculation(row, column, recursive)](/cells/zh/python-net/aspose.cells/cells/get_dependents_in_calculation/#int-int-bool) |获取计算结果取决于特定单元格的所有单元格。|
| [get_cell_style(row, column)](/cells/zh/python-net/aspose.cells/cells/get_cell_style/#int-int) |获取给定单元格的样式。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
* 类 [Column](/cells/zh/python-net/aspose.cells/column)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
* 类 [Row](/cells/zh/python-net/aspose.cells/row)
