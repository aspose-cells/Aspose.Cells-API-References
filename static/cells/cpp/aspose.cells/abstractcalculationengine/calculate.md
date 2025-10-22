##Aspose::Cells::AbstractCalculationEngine::Calculate method
'Aspose::Cells::AbstractCalculationEngine::Calculate method. Calculates one function with given data in C++.'
## AbstractCalculationEngine::Calculate method
Calculates one function with given data.
```cpp
virtual void Aspose::Cells::AbstractCalculationEngine::Calculate(CalculationData &data)=0
```
| Parameter | Type | Description |
| --- | --- | --- |
| data | CalculationData\& | the required data to calculate function such as function name, parameters, ...etc. |
## Remarks
User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.
## See Also
* Class [CalculationData](../../calculationdata/)
* Class [AbstractCalculationEngine](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
