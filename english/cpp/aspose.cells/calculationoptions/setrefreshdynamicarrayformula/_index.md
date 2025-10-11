---
title: Aspose::Cells::CalculationOptions::SetRefreshDynamicArrayFormula method
linktitle: SetRefreshDynamicArrayFormula
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions::SetRefreshDynamicArrayFormula method. Indicates whether dynamic array formulas should be refreshed before calculating formulas in C++.'
type: docs
weight: 1200
url: /cpp/aspose.cells/calculationoptions/setrefreshdynamicarrayformula/
---
## CalculationOptions::SetRefreshDynamicArrayFormula method


Indicates whether dynamic array formulas should be refreshed before calculating formulas.

```cpp
void Aspose::Cells::CalculationOptions::SetRefreshDynamicArrayFormula(bool value)
```

## Remarks


If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise(UserSpecifiedRefreshDynamicArrayFormula is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as Workbook.CalculateFormula(CalculationOptions), this property will be taken as true. For other cases, such as Cell.Calculate(CalculationOptions) or Worksheet.CalculateFormula(CalculationOptions, bool), this property will be taken as false. 
## See Also

* Class [CalculationOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
