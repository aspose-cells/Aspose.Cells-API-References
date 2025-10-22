##Aspose::Cells::CalculationOptions::SetRefreshDynamicArrayFormula method
'Aspose::Cells::CalculationOptions::SetRefreshDynamicArrayFormula method. Indicates whether dynamic array formulas should be refreshed before calculating formulas in C++.'
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
