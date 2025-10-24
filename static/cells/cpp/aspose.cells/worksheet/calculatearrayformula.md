##Aspose::Cells::Worksheet::CalculateArrayFormula method
'Aspose::Cells::Worksheet::CalculateArrayFormula method. Calculates a formula as array formula in C++.'
## Worksheet::CalculateArrayFormula(const U16String\&, const CalculationOptions\&) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const U16String &formula, const CalculationOptions &opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [U16String](../../u16string/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateArrayFormula(const char16_t*, const CalculationOptions\&) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const char16_t *formula, const CalculationOptions &opts)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateArrayFormula(const U16String\&, const CalculationOptions\&, int32_t, int32_t) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const U16String &formula, const CalculationOptions &opts, int32_t maxRowCount, int32_t maxColumnCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
| maxRowCount | int32_t | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | int32_t | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
## ReturnValue
Calculated formula result.
## Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [U16String](../../u16string/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateArrayFormula(const char16_t*, const CalculationOptions\&, int32_t, int32_t) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const char16_t *formula, const CalculationOptions &opts, int32_t maxRowCount, int32_t maxColumnCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
| opts | const CalculationOptions\& | Options for calculating formula |
| maxRowCount | int32_t | the maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | int32_t | the maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
## ReturnValue
Calculated formula result.
## Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateArrayFormula(const U16String\&, const FormulaParseOptions\&, const CalculationOptions\&, int32_t, int32_t, int32_t, int32_t, const CalculationData\&) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const U16String &formula, const FormulaParseOptions &pOpts, const CalculationOptions &cOpts, int32_t baseCellRow, int32_t baseCellColumn, int32_t maxRowCount, int32_t maxColumnCount, const CalculationData &calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const U16String\& | Formula to be calculated. |
| pOpts | const FormulaParseOptions\& | Options for parsing formula |
| cOpts | const CalculationOptions\& | Options for calculating formula |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
| maxRowCount | int32_t | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | int32_t | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | const CalculationData\& | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for AbstractCalculationEngine.Calculate(CalculationData). |
## ReturnValue
Calculated formula result.
## Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [U16String](../../u16string/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [CalculationData](../../calculationdata/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## Worksheet::CalculateArrayFormula(const char16_t*, const FormulaParseOptions\&, const CalculationOptions\&, int32_t, int32_t, int32_t, int32_t, const CalculationData\&) method
Calculates a formula as array formula.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::Worksheet::CalculateArrayFormula(const char16_t *formula, const FormulaParseOptions &pOpts, const CalculationOptions &cOpts, int32_t baseCellRow, int32_t baseCellColumn, int32_t maxRowCount, int32_t maxColumnCount, const CalculationData &calculationData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | const char16_t* | Formula to be calculated. |
| pOpts | const FormulaParseOptions\& | Options for parsing formula |
| cOpts | const CalculationOptions\& | Options for calculating formula |
| baseCellRow | int32_t | The row index of the base cell. |
| baseCellColumn | int32_t | The column index of the base cell. |
| maxRowCount | int32_t | The maximum row count of resultant data. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | int32_t | The maximum column count of resultant data. If it is non-positive or greater than the actual row count, then actual column count will be used. |
| calculationData | const CalculationData\& | The calculation data. It is used for the situation that user needs to calculate some static formulas when implementing custom calculation engine. For such kind of situation, user needs to specify it with the calculation data provided for AbstractCalculationEngine.Calculate(CalculationData). |
## ReturnValue
Calculated formula result.
## Remarks
The formula will be taken as dynamic array formula to calculate the dimension and result. User specified maximum dimension is used for cases that the calculated result is large data set (for example, the calculated result may correspond to a whole row or column data) but user does not need so large an array according to business requirement or for performance consideration.
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [FormulaParseOptions](../../formulaparseoptions/)
* Class [CalculationOptions](../../calculationoptions/)
* Class [CalculationData](../../calculationdata/)
* Class [Worksheet](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
