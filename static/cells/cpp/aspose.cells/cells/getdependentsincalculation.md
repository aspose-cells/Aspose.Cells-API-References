##Aspose::Cells::Cells::GetDependentsInCalculation method
'Aspose::Cells::Cells::GetDependentsInCalculation method. Gets all cells whose calculated result depends on specific cell in C++.'
## Cells::GetDependentsInCalculation method
Gets all cells whose calculated result depends on specific cell.
```cpp
Enumerator<Cell> Aspose::Cells::Cells::GetDependentsInCalculation(int32_t row, int32_t column, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | int32_t | [Row](../../row/) index of the specific cell |
| column | int32_t | [Column](../../column/) index of the specific cell. |
| recursive | bool | Whether returns those dependents which do not reference to the specific cell directly but reference to other leafs of that cell. |
## ReturnValue
[Enumerator](../../enumerator/) to enumerate all dependents(Cell objects)
## Remarks
To use this method, please make sure the workbook has been set with true value for FormulaSettings.EnableCalculationChain and has been fully calculated with this setting. If there is no formula reference to this cell, null will be returned. For more details and example, please see [Cell.GetDependentsInCalculation(bool)](../../cell/getdependentsincalculation/)
## See Also
* Class [Enumerator](../../enumerator/)
* Class [Cell](../../cell/)
* Class [Vector](../../vector/)
* Class [Cells](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
