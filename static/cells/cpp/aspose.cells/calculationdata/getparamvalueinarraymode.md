##Aspose::Cells::CalculationData::GetParamValueInArrayMode method
'Aspose::Cells::CalculationData::GetParamValueInArrayMode method. Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode in C++.'
## CalculationData::GetParamValueInArrayMode method
Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.
```cpp
Vector<Vector<Aspose::Cells::Object>> Aspose::Cells::CalculationData::GetParamValueInArrayMode(int32_t index, int32_t maxRowCount, int32_t maxColumnCount)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index of the parameter(0 based) |
| maxRowCount | int32_t | The row count limit for the returned array. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | int32_t | The column count limit for the returned array. If it is non-positive or greater than the actual row count, then actual column count will be used. |
## ReturnValue
An array which contains all items represented by the specified parameter.
## Remarks
For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to Cells.MaxDataRow and Cells.MaxDataColumn), otherwise the returned large array may increase memory cost with large amount of useless data.
## See Also
* Class [Vector](../../vector/)
* Class [Object](../../object/)
* Class [CalculationData](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
