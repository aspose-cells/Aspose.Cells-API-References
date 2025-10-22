##Aspose::Cells::Cell::SetDynamicArrayFormula method
'Aspose::Cells::Cell::SetDynamicArrayFormula method. Sets dynamic array formula and make the formula spill into neighboring cells if possible in C++.'
## Cell::SetDynamicArrayFormula(const U16String\&, const FormulaParseOptions\&, bool) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const U16String &arrayFormula, const FormulaParseOptions &options, bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const U16String\& | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const char16_t*, const FormulaParseOptions\&, bool) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const char16_t *arrayFormula, const FormulaParseOptions &options, bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const char16_t* | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const U16String\&, const FormulaParseOptions\&, const Vector \<Vector \<Aspose::Cells::Object\>\>\&, bool, bool) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const U16String &arrayFormula, const FormulaParseOptions &options, const Vector<Vector<Aspose::Cells::Object>> &values, bool calculateRange, bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const U16String\& | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | const Vector \<Vector \<Aspose::Cells::Object\>\>\& | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | bool | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const char16_t*, const FormulaParseOptions\&, const Vector \<Vector \<Aspose::Cells::Object\>\>\&, bool, bool) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const char16_t *arrayFormula, const FormulaParseOptions &options, const Vector<Vector<Aspose::Cells::Object>> &values, bool calculateRange, bool calculateValue)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const char16_t* | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | const Vector \<Vector \<Aspose::Cells::Object\>\>\& | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | bool | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const U16String\&, const FormulaParseOptions\&, const Vector \<Vector \<Aspose::Cells::Object\>\>\&, bool, bool, const CalculationOptions\&) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const U16String &arrayFormula, const FormulaParseOptions &options, const Vector<Vector<Aspose::Cells::Object>> &values, bool calculateRange, bool calculateValue, const CalculationOptions &copts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const U16String\& | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | const Vector \<Vector \<Aspose::Cells::Object\>\>\& | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | bool | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | const CalculationOptions\& | The options for calculating formula. Commonly, for performance consideration, the CalculationOptions.Recursive property should be false. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Cell::SetDynamicArrayFormula(const char16_t*, const FormulaParseOptions\&, const Vector \<Vector \<Aspose::Cells::Object\>\>\&, bool, bool, const CalculationOptions\&) method
Sets dynamic array formula and make the formula spill into neighboring cells if possible.
```cpp
CellArea Aspose::Cells::Cell::SetDynamicArrayFormula(const char16_t *arrayFormula, const FormulaParseOptions &options, const Vector<Vector<Aspose::Cells::Object>> &values, bool calculateRange, bool calculateValue, const CalculationOptions &copts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| arrayFormula | const char16_t* | the formula expression |
| options | const FormulaParseOptions\& | options to parse formula. "Parse" option will be ignored and the formula will always be parsed immediately |
| values | const Vector \<Vector \<Aspose::Cells::Object\>\>\& | values(calculated results) for those cells with given dynamic array formula |
| calculateRange | bool | Whether calculate the spilled range for this dynamic array formula. If the "values" parameter is not null and this flag is false, then the spilled range's height will be values.Length and width will be values[0].Length. |
| calculateValue | bool | whether calculate this dynamic array formula for those cells in the spilled range when "values" is null or corresponding item in "values" for one cell is null. |
| copts | const CalculationOptions\& | The options for calculating formula. Commonly, for performance consideration, the CalculationOptions.Recursive property should be false. |
## ReturnValue
the range that the formula should spill into.
## Remarks
the returned range may be not same with the actual one that this dynamic array formula spills into. If there are non-empty cells in the range, the formula will be set for current cell only and marked as "#SPILL!". But for such kind of situation we still return the whole range that this formula should spill into.
## See Also
* Class [CellArea](../../cellarea/)
* Class [Vector](../../vector/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [Object](../../object/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Cell](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
