---
title: "PivotField.Subtotals"
second_title: "Aspose.Cells 的 .NET API 参考"
description: "PivotField 属性。获取或设置字段的子总计。仅适用于行或列透视字段"
type: docs
url: /zh/net/aspose.cells.pivot/pivotfield/subtotals/
---
## PivotField.Subtotals property

获取或设置字段的子总计。仅适用于行或列透视字段。

```csharp
public PivotFieldSubtotalType Subtotals { get; set; }
```

### 示例

```csharp

[C#]
//无小计
rowField.Subtotals = PivotFieldSubtotalType.None;
//自动小计
//rowField.Subtotals = PivotFieldSubtotalType.Automatic;
//单个小计：求和
//rowField.Subtotals = PivotFieldSubtotalType.Sum;
//多重小计：求和和计数数字
//rowField.Subtotals = PivotFieldSubtotalType.Sum | PivotFieldSubtotalType.Count;
```

### 另请参见

* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


