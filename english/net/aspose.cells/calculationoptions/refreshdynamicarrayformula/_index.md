---
title: CalculationOptions.RefreshDynamicArrayFormula
second_title: Aspose.Cells for .NET API Reference
description: CalculationOptions property. Indicates whether dynamic array formulas should be refreshed before calculating formulas
type: docs
url: /net/aspose.cells/calculationoptions/refreshdynamicarrayformula/
---
## CalculationOptions.RefreshDynamicArrayFormula property

Indicates whether dynamic array formulas should be refreshed before calculating formulas.

```csharp
public bool RefreshDynamicArrayFormula { get; set; }
```

### Remarks

If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([`UserSpecifiedRefreshDynamicArrayFormula`](../userspecifiedrefreshdynamicarrayformula/) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [`CalculateFormula`](../../workbook/calculateformula/), this property will be taken as true. For other cases, such as [`Calculate`](../../cell/calculate/) or [`CalculateFormula`](../../worksheet/calculateformula/), this property will be taken as false.

### See Also

* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


