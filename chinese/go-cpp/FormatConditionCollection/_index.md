---
title: "FormatConditionCollection 类"
linktitle: "FormatConditionCollection"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "FormatConditionCollection 类。封装在 Go 中表示 formatconditioncollection 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/formatconditioncollection/
---

## FormatConditionCollection class

表示条件格式化。FormatConditions 可以包含最多三个条件格式。

```go

type FormatConditionCollection struct  {
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
| [Add](./add/) | 向 FormatConditions 添加一个格式条件和受影响的单元格范围。FormatConditions 最多可以包含三个条件格式。条件格式的公式中不允许引用其他工作表。 |
| [AddArea](./addarea/) | 添加一个条件格式化的单元格范围。 |
| [AddCondition_FormatConditionType_OperatorType_String_String](./addcondition_formatconditiontype_operatortype_string_string/) | 添加一个格式条件。 |
| [AddCondition_FormatConditionType](./addcondition_formatconditiontype/) | 添加格式条件。 |
| [GetCount](./getcount/) | 获取条件的计数。 |
| [GetRangeCount](./getrangecount/) | 获取条件格式化范围的计数。 |
| [Get](./get/) | 按索引获取格式条件。 |
| [GetCellArea](./getcellarea/) | 按索引获取条件格式化的单元格范围。 |
| [RemoveArea_Int](./removearea_int/) | 按索引移除条件格式化的单元格范围。 |
| [RemoveArea_Int_Int_Int_Int](./removearea_int_int_int_int/) | 在范围内移除条件格式。 |
| [RemoveCondition](./removecondition/) | 按索引移除格式条件。 |
