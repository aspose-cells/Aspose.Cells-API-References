---
title: CellsHelper class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 230
url: /python-net/aspose.cells/cellshelper/
is_root: false
---

## CellsHelper class

Provides helper functions.



The CellsHelper type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [significant_digits](/cells/python-net/aspose.cells/cellshelper/significant_digits) | Gets and sets the number of significant digits.<br/>The default value is 17. |
| [dpi](/cells/python-net/aspose.cells/cellshelper/dpi) | Gets the DPI of the machine. |
| [startup_path](/cells/python-net/aspose.cells/cellshelper/startup_path) | Gets or sets the startup path, which is referred to by some external formula references. |
| [alt_start_path](/cells/python-net/aspose.cells/cellshelper/alt_start_path) | Gets or sets the alternate startup path, which is referred to by some external formula references. |
| [library_path](/cells/python-net/aspose.cells/cellshelper/library_path) | Gets or sets the library path which is referred to by some external formula references. |
| [custom_implementation_factory](/cells/python-net/aspose.cells/cellshelper/custom_implementation_factory) | Gets or sets the factory for creating instances with special implementation. |
| [is_cloud_platform](/cells/python-net/aspose.cells/cellshelper/is_cloud_platform) | Please set this property True when running on a cloud platform, such as: Azure, AWSLambda, etc, |


### Methods
| Method | Description |
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) | Checks given sheet name and create a valid one when needed.<br/>If given sheet name conforms to the rules of excel sheet name, then return it.<br/>Otherwise string will be truncated if length exceeds the limit<br/>and invalid characters will be replaced with ' ', then return the rebuilt string value. |
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) | Checks given sheet name and create a valid one when needed.<br/>If given sheet name conforms to the rules of excel sheet name, then return it.<br/>Otherwise string will be truncated if length exceeds the limit<br/>and invalid characters will be replaced with given character, then return the rebuilt string value. |
| [get_text_width(text, font, scaling)](/cells/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) | Get width of text in unit of points. |
| [get_version()](/cells/python-net/aspose.cells/cellshelper/get_version/#) | Get the release version. |
| [cell_name_to_index(cell_name, row, column)](/cells/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) | Gets the cell row and column indexes according to its name. |
| [cell_index_to_name(row, column)](/cells/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) | Gets cell name according to its row and column indexes. |
| [column_index_to_name(column)](/cells/python-net/aspose.cells/cellshelper/column_index_to_name/#int) | Gets column name according to column index. |
| [column_name_to_index(column_name)](/cells/python-net/aspose.cells/cellshelper/column_name_to_index/#str) | Gets column index according to column name. |
| [row_index_to_name(row)](/cells/python-net/aspose.cells/cellshelper/row_index_to_name/#int) | Gets row name according to row index. |
| [row_name_to_index(row_name)](/cells/python-net/aspose.cells/cellshelper/row_name_to_index/#str) | Gets row index according to row name. |
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) | Converts the r1c1 formula of the cell to A1 formula. |
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) | Converts A1 formula of the cell to the r1c1 formula. |
| [get_date_time_from_double(double_value, date1904)](/cells/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) | Convert the double value to the date time value. |
| [get_double_from_date_time(date_time, date1904)](/cells/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) | Convert the date time to double value. |
| [get_used_colors(workbook)](/cells/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) | Gets all used colors in the workbook. |
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) | Add addin function. |
| [merge_files(files, cached_file, dest_file)](/cells/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) | Merges some large xls files to a xls file. |
| [init_for_dot_net_core()](/cells/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) | Do the initialization for .NetCore programme.<br/>We suggest you to call this method for all .NetCore initialization first. <br/>For example:<br/>CellsHelper.InitForDotNetCore();<br/>Workbook wb = new Workbook(); |


### See Also

* module [aspose.cells](../)
