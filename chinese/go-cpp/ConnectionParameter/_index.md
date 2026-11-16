---
title: "ConnectionParameter 类"
linktitle: "ConnectionParameter"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ConnectionParameter 类。封装在 Go 中表示 connectionparameter 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/connectionparameter/
---

## ConnectionParameter class

指定外部数据连接使用的任何参数的属性，这些参数适用于 ODBC 和 Web 查询。

```go

type ConnectionParameter struct  {
	ptr unsafe.Pointer
}

```
## 构造函数

| 方法 | 描述 |
| --- | --- |

## 方法

| 方法 | 描述 |
| --- | --- |
| [IsNull](./isnull/) | 检查实现对象是否为 nullptr。 |
| [GetSqlType](./getsqltype/) | 参数的 SQL 数据类型。仅对 ODBC 源有效。 |
| [SetSqlType](./setsqltype/) | 参数的 SQL 数据类型。仅对 ODBC 源有效。 |
| [GetRefreshOnChange](./getrefreshonchange/) | 标志指示查询是否应在提供参数值的单元格内容更改时自动刷新。如果为 true，则每次更改时都会使用新的参数值刷新外部数据。如果为 false，则仅在用户请求或其他事件触发刷新时（例如打开工作簿）刷新外部数据。 |
| [SetRefreshOnChange](./setrefreshonchange/) | 标志指示查询是否应在提供参数值的单元格内容更改时自动刷新。如果为 true，则每次更改时都会使用新的参数值刷新外部数据。如果为 false，则仅在用户请求或其他事件触发刷新时（例如打开工作簿）刷新外部数据。 |
| [GetPrompt](./getprompt/) | 参数的提示字符串。与输入 UI 一起呈现给电子表格用户，以在刷新外部数据之前收集参数值。仅在 parameterType = prompt 时使用。 |
| [SetPrompt](./setprompt/) | 参数的提示字符串。与输入 UI 一起呈现给电子表格用户，以在刷新外部数据之前收集参数值。仅在 parameterType = prompt 时使用。 |
| [GetType](./gettype/) | 使用的参数类型。如果 parameterType = value，则使用布尔、双精度、整数或字符串中的值。在这种情况下，预计只会指定 {boolean、double、integer 或 string} 中的一个。 |
| [SetType](./settype/) | 使用的参数类型。如果 parameterType = value，则使用布尔、双精度、整数或字符串中的值。在这种情况下，预计只会指定 {boolean、double、integer 或 string} 中的一个。 |
| [GetName](./getname/) | 参数的名称。 |
| [SetName](./setname/) | 参数的名称。 |
| [GetCellReference](./getcellreference/) | 单元格引用，指示用于查询参数的单元格值。仅在 parameterType 为 cell 时使用。 |
| [SetCellReference](./setcellreference/) | 单元格引用，指示用于查询参数的单元格值。仅在 parameterType 为 cell 时使用。 |
| [GetValue](./getvalue/) | 非整数数值、整数值、字符串值或布尔值，用作查询参数。仅在 parameterType 为 value 时使用。 |
| [SetValue](./setvalue/) | 非整数数值、整数值、字符串值或布尔值，用作查询参数。仅在 parameterType 为 value 时使用。 |
