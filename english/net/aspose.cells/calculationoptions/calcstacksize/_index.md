---
title: CalculationOptions.CalcStackSize
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. The stack size for calculating cells recursively. Default value is 200
type: docs
url: /net/aspose.cells/calculationoptions/calcstacksize/
---
## CalculationOptions.CalcStackSize property

The stack size for calculating cells recursively. Default value is 200.

```csharp
public int CalcStackSize { get; set; }
```

### Remarks

When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. However, too small value may cause performance degradation for the formula calculation and value less than 2 will make it impossible to calculate formula which depends on another one. So if the specified value is less than 2, it will be reset to 2.

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


