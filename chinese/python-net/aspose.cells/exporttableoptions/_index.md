---
title: ExportTableOptions类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 550
url: /zh/python-net/aspose.cells/exporttableoptions/
is_root: false
---
## ExportTableOptions类
表示所有导出表选项。



ExportTableOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [ExportTableOptions()](/cells/zh/python-net/aspose.cells/exporttableoptions/__init__/#) |构造一个新的 ExportTableOptions 实例|


### 特性
|属性|描述|
| :- | :- |
| [export_column_name](/cells/zh/python-net/aspose.cells/exporttableoptions/export_column_name) |表示第一行的数据是否导出到DataTable的列名。<br/>默认值为假。|
| [skip_error_value](/cells/zh/python-net/aspose.cells/exporttableoptions/skip_error_value) |指示是否跳过列的无效值。<br/>例如，如果列类型为 decimal ，则该值大于 decimal.MaxValue<br/>并且此属性为真，我们不会再抛出异常。<br/>默认值为假。|
| [plot_visible_cells](/cells/zh/python-net/aspose.cells/exporttableoptions/plot_visible_cells) |仅导出可见单元格。|
| [plot_visible_rows](/cells/zh/python-net/aspose.cells/exporttableoptions/plot_visible_rows) |仅导出可见行。|
| [plot_visible_columns](/cells/zh/python-net/aspose.cells/exporttableoptions/plot_visible_columns) |仅导出可见列。|
| [export_as_string](/cells/zh/python-net/aspose.cells/exporttableoptions/export_as_string) |将单元格的字符串值导出到 DataTable。|
| [export_as_html_string](/cells/zh/python-net/aspose.cells/exporttableoptions/export_as_html_string) |将单元格的 html 字符串值导出到 DataTable。|
| [format_strategy](/cells/zh/python-net/aspose.cells/exporttableoptions/format_strategy) |获取和设置将值导出为字符串值时的格式策略。|
| [check_mixed_value_type](/cells/zh/python-net/aspose.cells/exporttableoptions/check_mixed_value_type) | False，Aspose.Cells 将根据第一行的值类型设置 DataColumn 的类型以提高性能。<br/> True, Aspose.Cells 会在设置DataColumn的类型前检查列中的值类型是否混合<br/>和值类型混合，DataColumn 的类型将是字符串。|
| [is_vertical](/cells/zh/python-net/aspose.cells/exporttableoptions/is_vertical) |如果 Workbook 文件中的一行代表 DataTable 中的一行，则为真。如果 Workbook 文件中的列代表 DataTable 中的一行，则为 False。|
| [indexes](/cells/zh/python-net/aspose.cells/exporttableoptions/indexes) |应导出的列/行的索引。|
| [rename_strategy](/cells/zh/python-net/aspose.cells/exporttableoptions/rename_strategy) |列重复名称的策略。|



### 也可以看看
* 模块 [aspose.cells](..)
