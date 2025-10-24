##Aspose::Cells::CalculationData::GetCell method
'Aspose::Cells::CalculationData::GetCell method. Gets the Cell object where the function is in in C++.'
## CalculationData::GetCell method
Gets the [Cell](../../cell/) object where the function is in.
```cpp
Cell Aspose::Cells::CalculationData::GetCell()
```
## Remarks
When calculating a formula without setting it to a cell, such as by Worksheet.CalculateFormula(string, CalculationOptions), the formula will be calculated just like it has been set to cell A1, so both CellRow and CellColumn are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.
## See Also
* Class [Cell](../../cell/)
* Class [CalculationData](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
