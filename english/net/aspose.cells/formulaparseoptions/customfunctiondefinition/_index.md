---
title: FormulaParseOptions.CustomFunctionDefinition
second_title: Aspose.Cells for .NET API Reference
description: FormulaParseOptions property. Definition for parsing custom functions
type: docs
url: /net/aspose.cells/formulaparseoptions/customfunctiondefinition/
---
## FormulaParseOptions.CustomFunctionDefinition property

Definition for parsing custom functions.

```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```

### Remarks

For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) to get the same result.

### See Also

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


