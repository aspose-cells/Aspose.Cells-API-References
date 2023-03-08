---
title: GlobalizationSettings类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 730
url: /zh/python-net/aspose.cells/globalizationsettings/
is_root: false
---
##  GlobalizationSettings类
代表全球化设置。



GlobalizationSettings 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [GlobalizationSettings()](/cells/zh/python-net/aspose.cells/globalizationsettings/__init__/#) |构造一个新的 GlobalizationSettings 实例|


### 特性
|属性|描述|
| :- | :- |
| [chart_settings](/cells/zh/python-net/aspose.cells/globalizationsettings/chart_settings) |获取或设置 Chart 的全球化设置。|
| [pivot_settings](/cells/zh/python-net/aspose.cells/globalizationsettings/pivot_settings) |获取或设置数据透视表的全球化设置。|
| [list_separator](/cells/zh/python-net/aspose.cells/globalizationsettings/list_separator) |获取列表分隔符、函数参数等。|
| [row_separator_of_formula_array](/cells/zh/python-net/aspose.cells/globalizationsettings/row_separator_of_formula_array) |获取公式中数组数据中行的分隔符。|
| [column_separator_of_formula_array](/cells/zh/python-net/aspose.cells/globalizationsettings/column_separator_of_formula_array) |获取公式中数组行数据中项目的分隔符。|


### 方法
|方法|描述|
| :- | :- |
| [get_pivot_total_name()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_pivot_total_name/#) |获取数据透视表中“总计”标签的名称。<br/>当数据透视表的数据区域中包含两个或多个数据透视字段时，您需要重写此方法。|
| [get_pivot_grand_total_name()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_pivot_grand_total_name/#) |获取数据透视表中“总计”标签的名称。|
| [get_multiple_items_name()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_multiple_items_name/#) |获取数据透视表中“（多项）”标签的名称。|
| [get_all_name()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_all_name/#) |获取数据透视表中“（全部）”标签的名称。|
| [get_protection_name_of_pivot_table()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_protection_name_of_pivot_table/#) |获取数据透视表中的保护名称。|
| [get_column_labels_of_pivot_table()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_column_labels_of_pivot_table/#) |获取数据透视表中“列标签”标签的名称。|
| [get_row_labels_name_of_pivot_table()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_row_labels_name_of_pivot_table/#) |获取数据透视表中“Row Labels”标签的名称。|
| [get_empty_data_name()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_empty_data_name/#) |获取数据透视表中“（空白）”标签的名称。|
| [get_data_field_header_name_of_pivot_table()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_data_field_header_name_of_pivot_table/#) |获取数据透视表中值区域字段标题的名称。|
| [get_sub_total_name(sub_total_type)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_sub_total_name/#aspose.cells.pivot.PivotFieldSubtotalType) |获取数据透视表中 [PivotFieldSubtotalType](/cells/zh/python-net/aspose.cells.pivot/pivotfieldsubtotaltype) 类型的名称。|
| [get_total_name(function_type)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_total_name/#ConsolidationFunction) |获取函数的总名称。|
| [get_grand_total_name(function_type)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_grand_total_name/#ConsolidationFunction) |获取函数的总计名称。|
| [get_table_row_type_of_headers()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_headers/#) |获取由表头组成的表行的类型名称。<br/>默认是“Headers”，所以在公式中“#Headers”代表表头。|
| [get_table_row_type_of_data()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_data/#) |获取由引用表的数据区域组成的表行的类型名称。<br/>默认是“数据”，所以在公式中“#Data”代表表格的数据区域。|
| [get_table_row_type_of_all()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_all/#) |获取由引用表中的所有行组成的表行的类型名称。<br/>默认值为“全部”，因此在公式中“#All”表示引用表中的所有行。|
| [get_table_row_type_of_totals()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_totals/#) |获取由引用表的总行组成的表行的类型名称。<br/>默认为“总计”，因此在公式中“#Totals”表示引用表的总行。|
| [get_table_row_type_of_current()](/cells/zh/python-net/aspose.cells/globalizationsettings/get_table_row_type_of_current/#) |获取由引用表中的当前行组成的表行的类型名称。<br/>默认为“This Row”，因此在公式中“#This Row”表示引用表中的当前行。|
| [get_error_value_string(err)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_error_value_string/#str) |获取单元格错误值的显示字符串值|
| [get_boolean_value_string(bv)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_boolean_value_string/#bool) |获取单元格布尔值的显示字符串值|
| [get_local_function_name(standard_name)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_local_function_name/#str) |根据给定的标准函数名称获取依赖于语言环境的函数名称。|
| [get_standard_function_name(local_name)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_standard_function_name/#str) |根据给定的语言环境相关函数名称获取标准函数名称。|
| [get_local_built_in_name(standard_name)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_local_built_in_name/#str) |根据给定的标准文本获取内置名称的区域设置相关文本。|
| [get_standard_built_in_name(local_name)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_standard_built_in_name/#str) |根据给定的语言环境相关文本获取内置名称的标准文本。|
| [get_standard_header_footer_font_style_name(localfont_style_name)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_standard_header_footer_font_style_name/#str) |根据给定的语言环境字体样式名称获取页眉/页脚的标准英文字体样式名称（常规、粗体、斜体）。|
| [get_comment_title_name(type)](/cells/zh/python-net/aspose.cells/globalizationsettings/get_comment_title_name/#aspose.cells.rendering.CommentTitleType) |根据评论标题类型获取依赖于语言环境的评论标题名称。|
| [compare(v1, v2, ignore_case)](/cells/zh/python-net/aspose.cells/globalizationsettings/compare/#str-str-bool) |根据一定的排序规则比较两个字符串值。|



### 也可以看看
* 模块 [aspose.cells](..)
* 类 [PivotFieldSubtotalType](/cells/zh/python-net/aspose.cells.pivot/pivotfieldsubtotaltype)
