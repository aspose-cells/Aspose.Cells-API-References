##Aspose::Cells::AbstractCalculationEngine::IsParamArrayModeRequired method
'Aspose::Cells::AbstractCalculationEngine::IsParamArrayModeRequired method. Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating custom functions and user has not updated the definition for them (by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), this property needs to be set as true in C++.'
## AbstractCalculationEngine::IsParamArrayModeRequired method
Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If CalculationData.GetParamValueInArrayMode(int, int, int) is required when calculating custom functions and user has not updated the definition for them (by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)), this property needs to be set as true.
```cpp
virtual bool Aspose::Cells::AbstractCalculationEngine::IsParamArrayModeRequired()
```
## Remarks
If this custom calculation engine needs the parameter to be calculated in array mode, more stacks will be required to cache the tree for parameters and [Calculate()](../calculate/) method may be called recursively to calculate the parameter's value. For performance consideration, please keep this property as the default value(false) if there is no special requirement.
## See Also
* Class [AbstractCalculationEngine](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
