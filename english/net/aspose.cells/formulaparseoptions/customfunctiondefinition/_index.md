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

### Examples

```csharp
// Called: CustomFunctionDefinition = customFunctionDefinition
public static void FormulaParseOptions_Property_CustomFunctionDefinition()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();

            // Create a new CustomFunctionDefinition instance
            CustomFunctionDefinition customFunctionDefinition = new CustomFunctionDefinition();

            // Create a new FormulaParseOptions instance and set the CustomFunctionDefinition
            FormulaParseOptions formulaParseOptions = new FormulaParseOptions
            {
                CustomFunctionDefinition = customFunctionDefinition
            };

            // Add a worksheet to the workbook
            Worksheet worksheet = workbook.Worksheets[0];

            // Define a custom formula
            string customFormula = "=MY_CUSTOM_FUNCTION(A1, B1)";

            // Parse the custom formula using the FormulaParseOptions
            worksheet.Cells["C1"].Formula = customFormula;
            worksheet.Cells["C1"].SetFormula(customFormula, formulaParseOptions);

            // Save the workbook
            workbook.Save("CustomFunctionDefinitionExample.xlsx");
            workbook.Save("CustomFunctionDefinitionExample.pdf");
            return;
        }
```

### See Also

* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


