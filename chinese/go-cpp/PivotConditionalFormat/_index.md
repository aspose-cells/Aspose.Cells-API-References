---
title: "PivotConditionalFormat 类"
linktitle: "PivotConditionalFormat"
second_title: "Aspose.Cells for Go via C++ API 参考"
description: "PivotConditionalFormat 类。封装在 Go 中表示 pivotconditionalformat 的对象。"
type: docs
weight: 200
url: /zh/go-cpp/pivotconditionalformat/
---

## PivotConditionalFormat class

表示 PivotFormatCondition 集合中的 PivotTable 格式条件。

```go

type PivotConditionalFormat struct  {
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
| [GetCellAreas](./getcellareas/) | 获取此条件格式适用的所有单元格区域。 |
| [GetPivotAreas](./getpivotareas/) | 获取所有数据透视区域。 |
| [AddCellArea](./addcellarea/) | 基于数据透视表视图添加区域。 |
| [ApplyTo](./applyto/) | 将条件格式应用于范围。仅适用于数据区域。 |
| [AddFieldArea_PivotFieldType_String](./addfieldarea_pivotfieldtype_string/) | 添加数据透视字段的区域。 |
| [AddFieldArea_PivotFieldType_PivotField](./addfieldarea_pivotfieldtype_pivotfield/) | 添加数据透视字段的区域。 |
| [GetFormatConditions](./getformatconditions/) | 获取数据透视表条件格式的条件。 |
| [GetScopeType](./getscopetype/) | 获取并设置数据透视表条件格式的作用域类型。 |
| [SetScopeType](./setscopetype/) | 获取并设置数据透视表条件格式的作用域类型。 |
| [GetRuleType](./getruletype/) | 获取并设置数据透视表条件格式的规则类型。 |
| [SetRuleType](./setruletype/) | 获取并设置数据透视表条件格式的规则类型。 |
