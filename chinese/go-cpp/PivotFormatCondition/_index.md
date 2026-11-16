---
title: "PivotFormatCondition 类"
linktitle: "PivotFormatCondition"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotFormatCondition 类。封装在 Go 中表示 pivotformatcondition 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotformatcondition/
---

## PivotFormatCondition class

表示 PivotFormatCondition 集合中的 PivotTable 格式条件。

```go

type PivotFormatCondition struct  {
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
| [AddDataAreaCondition_String](./adddataareacondition_string/) | 在数据字段中添加 PivotTable 条件格式限制。 |
| [AddDataAreaCondition_PivotField](./adddataareacondition_pivotfield/) | 在数据字段中添加 PivotTable 条件格式限制。 |
| [AddRowAreaCondition_String](./addrowareacondition_string/) | 在行字段中添加数据透视表条件格式限制。 |
| [AddRowAreaCondition_PivotField](./addrowareacondition_pivotfield/) | 在行字段中添加数据透视表条件格式限制。 |
| [AddColumnAreaCondition_String](./addcolumnareacondition_string/) | 在列字段中添加数据透视表条件格式限制。 |
| [AddColumnAreaCondition_PivotField](./addcolumnareacondition_pivotfield/) | 在列字段中添加数据透视表条件格式限制。 |
| [SetConditionalAreas](./setconditionalareas/) | 设置 PivotFormatCondition 对象的条件区域。 |
| [GetScopeType](./getscopetype/) | 获取并设置数据透视表条件格式的作用域类型。 |
| [SetScopeType](./setscopetype/) | 获取并设置数据透视表条件格式的作用域类型。 |
| [GetRuleType](./getruletype/) | 获取并设置数据透视表条件格式的规则类型。 |
| [SetRuleType](./setruletype/) | 获取并设置数据透视表条件格式的规则类型。 |
| [GetFormatConditions](./getformatconditions/) | 获取数据透视表条件格式的条件。 |
