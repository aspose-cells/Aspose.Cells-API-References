---
title: Aspose::Cells::CalculationOptions::GetRefreshDynamicArrayFormula method
linktitle: GetRefreshDynamicArrayFormula
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::CalculationOptions::GetRefreshDynamicArrayFormula method. Indicates whether dynamic array formulas should be refreshed before calculating formulas in C++.'
type: docs
weight: 1100
url: /cpp/aspose.cells/calculationoptions/getrefreshdynamicarrayformula/
---
## CalculationOptions::GetRefreshDynamicArrayFormula method


Indicates whether dynamic array formulas should be refreshed before calculating formulas.

```cpp
bool Aspose::Cells::CalculationOptions::GetRefreshDynamicArrayFormula()
```

## Remarks


If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise(UserSpecifiedRefreshDynamicArrayFormula is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as Workbook.CalculateFormula(CalculationOptions), this property will be taken as true. For other cases, such as Cell.Calculate(CalculationOptions) or Worksheet.CalculateFormula(CalculationOptions, bool), this property will be taken as false. 
## See Also

* Class [CalculationOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
