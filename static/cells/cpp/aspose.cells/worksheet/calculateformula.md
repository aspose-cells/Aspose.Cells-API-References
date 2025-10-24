##Aspose::Cells::Worksheet::CalculateFormula method
'Aspose::Cells::Worksheet::CalculateFormula method. Calculates a formula in C++.'
## Worksheet::CalculateFormula(const U16String\&) method
Calculates a formula.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const U16String &formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
## ReturnValue
Calculated formula result.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const char16_t*) method
Calculates a formula.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const char16_t *formula)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
## ReturnValue
Calculated formula result.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const U16String\&, const CalculationOptions\&) method
Calculates a formula expression directly.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const U16String &formula, const CalculationOptions &opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
## ReturnValue
Calculated result of given formula. The returned object may be of possible types of Cell.Value, or [ReferredArea](../../referredarea/).
## Remarks
The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use CalculateArrayFormula(string, CalculationOptions) instead.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const char16_t*, const CalculationOptions\&) method
Calculates a formula expression directly.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const char16_t *formula, const CalculationOptions &opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
## ReturnValue
Calculated result of given formula. The returned object may be of possible types of Cell.Value, or [ReferredArea](../../referredarea/).
## Remarks
The formula will be calculated just like it has been set to cell A1. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use CalculateArrayFormula(string, CalculationOptions) instead.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const U16String\&, const FormulaParseOptions\&, const CalculationOptions\&, int32_t, int32_t, const CalculationData\&) method
Calculates a formula expression directly.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const U16String &formula, const FormulaParseOptions &pOpts, const CalculationOptions &cOpts, int32_t baseCellRow, int32_t baseCellColumn, const CalculationData &calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
| pOpts | const FormulaParseOptions\& | Options for parsing formula. |
| cOpts | const CalculationOptions\& | Options for calculating formula. |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
| calculationData | const CalculationData\& | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for AbstractCalculationEngine.Calculate(CalculationData). |
## ReturnValue
Calculated result of given formula. The returned object may be of possible types of Cell.Value, or [ReferredArea](../../referredarea/).
## Remarks
The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) instead.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [CalculationData](../../calculationdata/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const char16_t*, const FormulaParseOptions\&, const CalculationOptions\&, int32_t, int32_t, const CalculationData\&) method
Calculates a formula expression directly.
```cpp
Aspose::Cells::Object Aspose::Cells::Worksheet::CalculateFormula(const char16_t *formula, const FormulaParseOptions &pOpts, const CalculationOptions &cOpts, int32_t baseCellRow, int32_t baseCellColumn, const CalculationData &calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
| pOpts | const FormulaParseOptions\& | Options for parsing formula. |
| cOpts | const CalculationOptions\& | Options for calculating formula. |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
| calculationData | const CalculationData\& | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for AbstractCalculationEngine.Calculate(CalculationData). |
## ReturnValue
Calculated result of given formula. The returned object may be of possible types of Cell.Value, or [ReferredArea](../../referredarea/).
## Remarks
The formula will be calculated just like it has been set to the specified base cell. And the formula will be taken as normal formula. If you need the formula be calculated as an array formula and to get an array for the calculated result, please use CalculateArrayFormula(string, FormulaParseOptions, CalculationOptions, int, int, int, int, CalculationData) instead.
## See Also
* Class [Object](../../object/)
* Class [Vector](../../vector/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [CalculationData](../../calculationdata/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateFormula(const CalculationOptions\&, bool) method
Calculates all formulas in this worksheet.
```cpp
void Aspose::Cells::Worksheet::CalculateFormula(const CalculationOptions &options, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | const CalculationOptions\& | Options for calculation |
| recursive | bool | True means if the worksheet' cells depend on the cells of other worksheets, the dependent cells in other worksheets will be calculated too. False means all the formulas in the worksheet have been calculated and the values are right. |
## See Also
* Class [Vector](../../vector/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
