##Aspose::Cells::CalculationData::SetCalculatedValue method
'Aspose::Cells::CalculationData::SetCalculatedValue method. Gets or sets the calculated value for this function in C++.'
## CalculationData::SetCalculatedValue method
Gets or sets the calculated value for this function.
```cpp
void Aspose::Cells::CalculationData::SetCalculatedValue(const Aspose::Cells::Object &value)
```
## Remarks
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of Cell.Value, or array of such kind of values, or a [Range](../../range/), [Name](../../name/), [ReferredArea](../../referredarea/). Getting this property before setting value to it will make the function be calculated by the default calculation engine of [Aspose.Cells](../../) and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
## See Also
* Class [Object](../../object/)
* Class [CalculationData](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
