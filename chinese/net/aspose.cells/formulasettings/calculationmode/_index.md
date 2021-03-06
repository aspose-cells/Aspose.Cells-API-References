---
title: CalculationMode
second_title: Aspose.Cells for .NET API 参考
description: 获取或设置 ms excel 中工作簿计算的模式
type: docs
weight: 40
url: /zh/net/aspose.cells/formulasettings/calculationmode/
---
## FormulaSettings.CalculationMode property

获取或设置 ms excel 中工作簿计算的模式。

```csharp
public CalcModeType CalculationMode { get; set; }
```

### 评论

此属性仅用于将设置保存到生成的电子表格文件 所以其他应用程序（例如 ms excel）在加载和操作生成的文件时可能会采取相应的行动。 出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式， 无论为此属性设置了何种模式。 如果用户需要计算公式，请始终根据需要在不同的对象上调用方法: [`CalculateFormula`](../../workbook/calculateformula),[`CalculateFormula`](../../worksheet/calculateformula), [`Calculate`](../../cell/calculate), ...等。

### 也可以看看

* enum [CalcModeType](../../calcmodetype)
* class [FormulaSettings](../../formulasettings)
* 命名空间 [Aspose.Cells](../../formulasettings)
* 部件 [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
