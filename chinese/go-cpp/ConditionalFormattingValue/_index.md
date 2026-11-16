---
title: "ConditionalFormattingValue 类"
linktitle: "ConditionalFormattingValue"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "ConditionalFormattingValue 类。封装在 Go 中表示 conditionalformattingvalue 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/conditionalformattingvalue/
---

## ConditionalFormattingValue class

描述渐变比例、数据条或图标集中的插值点值。

```go

type ConditionalFormattingValue struct  {
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
| [GetValue](./getvalue/) | 获取或设置此条件格式值对象的值。应与 Type 一起使用。 |
| [SetValue](./setvalue/) | 获取或设置此条件格式值对象的值。应与 Type 一起使用。 |
| [GetType](./gettype/) | 获取或设置此条件格式值对象的类型。将类型设置为 FormatConditionValueType.Min 或 FormatConditionValueType.Max 将自动将 \"Value\" 设为 null。 |
| [SetType](./settype/) | 获取或设置此条件格式值对象的类型。将类型设置为 FormatConditionValueType.Min 或 FormatConditionValueType.Max 将自动将 \"Value\" 设为 null。 |
| [IsGTE](./isgte/) | 获取或设置“大于或等于”标志。仅用于图标集，决定此阈值是否使用“大于或等于”运算符。'false' 表示使用“大于”，而不是“大于或等于”。默认值为 true。 |
| [SetIsGTE](./setisgte/) | 获取或设置“大于或等于”标志。仅用于图标集，决定此阈值是否使用“大于或等于”运算符。'false' 表示使用“大于”，而不是“大于或等于”。默认值为 true。 |
