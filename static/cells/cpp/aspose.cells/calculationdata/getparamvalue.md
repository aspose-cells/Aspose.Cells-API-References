##Aspose::Cells::CalculationData::GetParamValue method
'Aspose::Cells::CalculationData::GetParamValue method. Gets the represented value object of the parameter at given index in C++.'
## CalculationData::GetParamValue method
Gets the represented value object of the parameter at given index.
```cpp
Aspose::Cells::Object Aspose::Cells::CalculationData::GetParamValue(int32_t index)
```
| Parameter | Type | Description |
| --- | --- | --- |
| index | int32_t | The index of the parameter(0 based) |
## ReturnValue
The calculated value of the parameter.
## Remarks
For one parameter:
If it is plain value, then returns the plain value itself;
If it is reference, then returns [ReferredArea](../../referredarea/) object;
If it references to dataset(s) with multiple values, then returns array of objects;
If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) or FormulaParseOptions.CustomFunctionDefinition), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....
## See Also
* Class [Object](../../object/)
* Class [CalculationData](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
