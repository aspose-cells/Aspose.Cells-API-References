##Aspose::Cells::AbstractCalculationEngine::IsParamLiteralRequired method
'Aspose::Cells::AbstractCalculationEngine::IsParamLiteralRequired method. Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false in C++.'
## AbstractCalculationEngine::IsParamLiteralRequired method
Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false.
```cpp
virtual bool Aspose::Cells::AbstractCalculationEngine::IsParamLiteralRequired()
```
## Remarks
If this custom calculation engine needs the parameter's literal text, more stacks will be required to cache the literal text for parameters and [Calculate()](../calculate/) method may be called recursively to calculate the parameter's value. Generally the literal text is not needed for calculating formulas and this property should be kept as false for most implementations to get better performance.
## See Also
* Class [AbstractCalculationEngine](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
