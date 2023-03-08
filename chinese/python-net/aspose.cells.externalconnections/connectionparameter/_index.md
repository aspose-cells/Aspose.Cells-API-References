---
title: ConnectionParameter类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 10
url: /zh/python-net/aspose.cells.externalconnections/connectionparameter/
is_root: false
---
##  ConnectionParameter类
指定有关用于外部数据连接的任何参数的属性
参数对 ODBC 和 Web 查询有效。



ConnectionParameter 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [sql_type](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/sql_type) |参数的 SQL 数据类型。仅对 ODBC 源有效。|
| [refresh_on_change](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/refresh_on_change) |指示查询是否应自动刷新内容的标志<br/>提供参数值更改的单元格。如果为真，则刷新外部数据<br/>每次有变化时使用新的参数值。如果为假，则为外部数据<br/>仅在用户请求时刷新，或某些其他事件触发刷新（例如，工作簿打开）。|
| [prompt](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/prompt) |参数的提示字符串。与输入 UI 一起呈现给电子表格用户<br/>在刷新外部数据之前收集参数值。仅在以下情况下使用<br/>参数类型 = 提示。|
| [type](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/type) |使用的参数类型。<br/>如果parameterType=value，那么value来自boolean, double, integer,<br/>或字符串将被使用。在这种情况下，预计只有一个<br/> {boolean, double, integer, or string} 将被指定。|
| [name](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/name) |参数的名称。|
| [cell_reference](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/cell_reference) | Cell 引用指示哪个单元格的值用于查询参数。仅当 parameterType 为 cell 时使用。|
| [value](/cells/zh/python-net/aspose.cells.externalconnections/connectionparameter/value) |非整数数值、整数值、字符串值或布尔值<br/>用作查询参数。仅在 parameterType 为 value 时使用。|



### 也可以看看
* 模块 [aspose.cells.externalconnections](..)
