##FormulaParseOptions.CustomFunctionDefinition
FormulaParseOptions property. Definition for parsing custom functions
## FormulaParseOptions.CustomFunctionDefinition property
Definition for parsing custom functions.
```csharp
public CustomFunctionDefinition CustomFunctionDefinition { get; set; }
```
### Remarks
For some special requirements, such as when calculating custom function in user's custom engine, some parameters of it need to be caculated in array mode, using this property can mark those parameters as array mode when parsing the formula. Otherwise user needs to update those custom functions later by [`UpdateCustomFunctionDefinition`](../../workbook/updatecustomfunctiondefinition/) to get the same result.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaParseOptionsPropertyCustomFunctionDefinitionDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create custom function definition
CustomFunctionDefinition customFunction = new CustomFunctionDefinition();
// Set up formula parse options with custom function
FormulaParseOptions options = new FormulaParseOptions
{
CustomFunctionDefinition = customFunction,
Parse = true
};
// Set sample data
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["B1"].PutValue(20);
// Use custom function in formula
string formula = "=MY_CUSTOM_FUNCTION(A1, B1)";
worksheet.Cells["C1"].SetFormula(formula, options);
// Calculate workbook to demonstrate custom function processing
workbook.CalculateFormula();
// Save result
workbook.Save("CustomFunctionDemo.xlsx");
}
}
}
```
### See Also
* class [CustomFunctionDefinition](../../customfunctiondefinition/)
* class [FormulaParseOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
