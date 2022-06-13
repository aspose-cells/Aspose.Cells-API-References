---
title: CalcStackSize
second_title: Aspose.Cells for .NET API 参考
description: 指定用于递归计算单元格的堆栈大小
type: docs
weight: 20
url: /zh/net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

指定用于递归计算单元格的堆栈大小。

```csharp
public int CalcStackSize { get; set; }
```

### 评论

当依赖树中有大量单元格需要递归计算时， StackOverflowException 可能在计算过程中引起。 如果是这样，用户应该为此属性指定较小的值。 对于这种情况，用户应根据实际的公式和数据确定该属性的合适值。 值太小可能导致公式计算性能下降。

### 也可以看看

* class [CalculationOptions](../../calculationoptions)
* 命名空间 [Aspose.Cells](../../calculationoptions)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->