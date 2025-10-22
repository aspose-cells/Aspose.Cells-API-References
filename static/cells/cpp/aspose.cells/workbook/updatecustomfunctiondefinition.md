##Aspose::Cells::Workbook::UpdateCustomFunctionDefinition method
'Aspose::Cells::Workbook::UpdateCustomFunctionDefinition method. Updates definition of custom functions in C++.'
## Workbook::UpdateCustomFunctionDefinition method
Updates definition of custom functions.
```cpp
void Aspose::Cells::Workbook::UpdateCustomFunctionDefinition(CustomFunctionDefinition *definition)
```
| Parameter | Type | Description |
| --- | --- | --- |
| definition | CustomFunctionDefinition* | Special definition of custom functions for user's special requirement. |
## Remarks
This method can be used for some special scenarios. For example, if user needs some parameters of some custom functions be calculated in array mode, then user may provide their own definition with implemented CustomFunctionDefinition.GetArrayModeParameters(string) for those functions. After the data of formulas being updated, those specified parameters will be calculated in array mode automatically when calculating corresponding custom functions.
## See Also
* Class [Vector](../../vector/)
* Class [CustomFunctionDefinition](../../customfunctiondefinition/)
* Class [Workbook](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
