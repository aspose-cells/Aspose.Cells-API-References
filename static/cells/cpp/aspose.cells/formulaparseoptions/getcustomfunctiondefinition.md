##Aspose::Cells::FormulaParseOptions::GetCustomFunctionDefinition method
'Aspose::Cells::FormulaParseOptions::GetCustomFunctionDefinition method. Definition for parsing custom functions in C++.'
## FormulaParseOptions::GetCustomFunctionDefinition method
Definition for parsing custom functions.
```cpp
CustomFunctionDefinition * Aspose::Cells::FormulaParseOptions::GetCustomFunctionDefinition()
```
## Remarks
For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) to get the same result.
## See Also
* Class [CustomFunctionDefinition](../../customfunctiondefinition/)
* Class [FormulaParseOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
