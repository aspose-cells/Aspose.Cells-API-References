##Aspose::Cells::CustomFunctionDefinition::GetArrayModeParameters method
'Aspose::Cells::CustomFunctionDefinition::GetArrayModeParameters method. Gets the indices of given custom function''s parameters that need to be calculated in array mode in C++.'
## CustomFunctionDefinition::GetArrayModeParameters(const U16String\&) method
Gets the indices of given custom function's parameters that need to be calculated in array mode.
```cpp
virtual Vector<int32_t> Aspose::Cells::CustomFunctionDefinition::GetArrayModeParameters(const U16String &functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | const U16String\& | [Name](../../name/) of the custom function. |
## ReturnValue
Indices of the parameters that need to be calculated in array mode for given custom function. Default is null, there is no parameter which needs to be calculated in array mode for the custom function.
## Remarks
For an expression that needs to be calculated, taking A:A+B:B as an example: Generally in value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used for the calculation.
## See Also
* Class [Vector](../../vector/)
* Class [U16String](../../u16string/)
* Class [CustomFunctionDefinition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
## CustomFunctionDefinition::GetArrayModeParameters(const char16_t*) method
Gets the indices of given custom function's parameters that need to be calculated in array mode.
```cpp
virtual Vector<int32_t> Aspose::Cells::CustomFunctionDefinition::GetArrayModeParameters(const char16_t *functionName)
```
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | const char16_t* | [Name](../../name/) of the custom function. |
## ReturnValue
Indices of the parameters that need to be calculated in array mode for given custom function. Default is null, there is no parameter which needs to be calculated in array mode for the custom function.
## Remarks
For an expression that needs to be calculated, taking A:A+B:B as an example: Generally in value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used for the calculation.
## See Also
* Class [Vector](../../vector/)
* Class [CustomFunctionDefinition](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
