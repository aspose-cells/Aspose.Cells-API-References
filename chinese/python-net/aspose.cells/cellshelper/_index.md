---
title: CellsHelper类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 230
url: /zh/python-net/aspose.cells/cellshelper/
is_root: false
---
## CellsHelper类
提供辅助函数。



CellsHelper 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [significant_digits](/cells/zh/python-net/aspose.cells/cellshelper/significant_digits) |获取和设置有效位数。<br/>默认值为 17。|
| [dpi](/cells/zh/python-net/aspose.cells/cellshelper/dpi) |获取机器的 DPI。|
| [startup_path](/cells/zh/python-net/aspose.cells/cellshelper/startup_path) |获取或设置启动路径，由一些外部公式引用引用。|
| [alt_start_path](/cells/zh/python-net/aspose.cells/cellshelper/alt_start_path) |获取或设置备用启动路径，该路径由某些外部公式引用引用。|
| [library_path](/cells/zh/python-net/aspose.cells/cellshelper/library_path) |获取或设置一些外部公式引用所引用的库路径。|
| [custom_implementation_factory](/cells/zh/python-net/aspose.cells/cellshelper/custom_implementation_factory) |获取或设置用于创建具有特殊实现的实例的工厂。|
| [is_cloud_platform](/cells/zh/python-net/aspose.cells/cellshelper/is_cloud_platform) |在云平台上运行时请将此属性设置为True，如：Azure、AWSLambda等，|


### 方法
|方法|描述|
| :- | :- |
| [create_safe_sheet_name(name_proposal)](/cells/zh/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str) |检查给定的工作表名称并在需要时创建有效的工作表名称。<br/>如果给定的工作表名称符合excel工作表名称的规则，则返回它。<br/>否则，如果长度超过限制，字符串将被截断<br/>无效字符将被替换为' '，然后返回重建的字符串值。|
| [create_safe_sheet_name(name_proposal, replace_char)](/cells/zh/python-net/aspose.cells/cellshelper/create_safe_sheet_name/#str-char) |检查给定的工作表名称并在需要时创建有效的工作表名称。<br/>如果给定的工作表名称符合excel工作表名称的规则，则返回它。<br/>否则，如果长度超过限制，字符串将被截断<br/>无效的字符将被替换为给定的字符，然后返回重建的字符串值。|
| [get_text_width(text, font, scaling)](/cells/zh/python-net/aspose.cells/cellshelper/get_text_width/#str-Font-float) |以点为单位获取文本的宽度。|
| [get_version()](/cells/zh/python-net/aspose.cells/cellshelper/get_version/#) |获取发布版本。|
| [cell_name_to_index(cell_name, row, column)](/cells/zh/python-net/aspose.cells/cellshelper/cell_name_to_index/#str-any-any) |根据其名称获取单元格的行和列索引。|
| [cell_index_to_name(row, column)](/cells/zh/python-net/aspose.cells/cellshelper/cell_index_to_name/#int-int) |根据其行和列索引获取单元格名称。|
| [column_index_to_name(column)](/cells/zh/python-net/aspose.cells/cellshelper/column_index_to_name/#int) |根据列索引获取列名。|
| [column_name_to_index(column_name)](/cells/zh/python-net/aspose.cells/cellshelper/column_name_to_index/#str) |根据列名获取列索引。|
| [row_index_to_name(row)](/cells/zh/python-net/aspose.cells/cellshelper/row_index_to_name/#int) |根据行索引获取行名。|
| [row_name_to_index(row_name)](/cells/zh/python-net/aspose.cells/cellshelper/row_name_to_index/#str) |根据行名获取行索引。|
| [convert_r1c1_formula_to_a1(r_1c1_formula, row, column)](/cells/zh/python-net/aspose.cells/cellshelper/convert_r1c1_formula_to_a1/#str-int-int) |将单元格的 r1c1 公式转换为 A1 公式。|
| [convert_a1_formula_to_r1c1(formula, row, column)](/cells/zh/python-net/aspose.cells/cellshelper/convert_a1_formula_to_r1c1/#str-int-int) |将单元格的 A1 公式转换为 r1c1 公式。|
| [get_date_time_from_double(double_value, date1904)](/cells/zh/python-net/aspose.cells/cellshelper/get_date_time_from_double/#float-bool) |将双精度值转换为日期时间值。|
| [get_double_from_date_time(date_time, date1904)](/cells/zh/python-net/aspose.cells/cellshelper/get_double_from_date_time/#DateTime-bool) |将日期时间转换为双精度值。|
| [get_used_colors(workbook)](/cells/zh/python-net/aspose.cells/cellshelper/get_used_colors/#Workbook) |获取工作簿中所有使用的颜色。|
| [add_add_in_function(function, min_count_of_parameters, max_count_of_parameters, paramers_type, function_value_type)](/cells/zh/python-net/aspose.cells/cellshelper/add_add_in_function/#str-int-int-list-ParameterType) |添加插件功能。|
| [merge_files(files, cached_file, dest_file)](/cells/zh/python-net/aspose.cells/cellshelper/merge_files/#list-str-str) |将一些大的 xls 文件合并为一个 xls 文件。|
| [init_for_dot_net_core()](/cells/zh/python-net/aspose.cells/cellshelper/init_for_dot_net_core/#) |对 .NetCore 程序进行初始化。<br/>我们建议您首先为所有 .NetCore 初始化调用此方法。<br/>例如：<br/>CellsHelper.InitForDotNetCore();<br/>工作簿 wb = new Workbook();|



### 也可以看看
* 模块 [aspose.cells](..)
