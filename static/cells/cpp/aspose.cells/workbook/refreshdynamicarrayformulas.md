##Aspose::Cells::Workbook::RefreshDynamicArrayFormulas method
'Aspose::Cells::Workbook::RefreshDynamicArrayFormulas method. Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas in C++.'
## Workbook::RefreshDynamicArrayFormulas(bool) method
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data) Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.
```cpp
void Aspose::Cells::Workbook::RefreshDynamicArrayFormulas(bool calculate)
```
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |
## See Also
* Class [Vector](../../vector/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Workbook::RefreshDynamicArrayFormulas(bool, const CalculationOptions\&) method
Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
```cpp
void Aspose::Cells::Workbook::RefreshDynamicArrayFormulas(bool calculate, const CalculationOptions &copts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |
| copts | const CalculationOptions\& | The options for calculating formulas |
## Remarks
For performance consideration, we do not refresh all dynamic array formulas automatically when the formula itself or the data it references to changed. So user need to call this method manually after those operations which may influence dynamic array formulas, such as importing/setting cell values, inserting/deleting rows/columns/ranges, ...etc.
For most formulas with functions, calculating the spill range also needs to calculating the formula, so in general true value for "calculate" flag is preferred. If the formula is simple, such as a range reference or array(for example "=C1:E5", "={1,2;3,4}", ...), simple function on a range or array(for example "=ABS(C1:E5)", "=1+{1,2;3,4}", ...), and all formulas will be calculated later(such as by Workbook.CalculateFormula(CalculationOptions)), then using false vlaue for "calculate" flag may avoid the duplicated calculation for the benefit of performance.
## See Also
* Class [Vector](../../vector/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
