---
title: Aspose::Cells::FormulaParseOptions::SetCustomFunctionDefinition method
linktitle: SetCustomFunctionDefinition
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::FormulaParseOptions::SetCustomFunctionDefinition method. Definition for parsing custom functions in C++.'
type: docs
weight: 1500
url: /cpp/aspose.cells/formulaparseoptions/setcustomfunctiondefinition/
---
## FormulaParseOptions::SetCustomFunctionDefinition method


Definition for parsing custom functions.

```cpp
void Aspose::Cells::FormulaParseOptions::SetCustomFunctionDefinition(CustomFunctionDefinition *value)
```

## Remarks


For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition) to get the same result. 
## See Also

* Class [Vector](../../vector/)
* Class [CustomFunctionDefinition](../../customfunctiondefinition/)
* Class [FormulaParseOptions](../)
* Namespace [Aspose::Cells](../../)
* Library [Aspose.Cells for C++](../../../)
