##Class CustomFunctionDefinition
Aspose.Cells.CustomFunctionDefinition class. Definition of custom function for calculating with users custom engine
## CustomFunctionDefinition class
Definition of custom function for calculating with user's custom engine.
```csharp
public class CustomFunctionDefinition
```
## Constructors
| Name | Description |
| --- | --- |
| [CustomFunctionDefinition](customfunctiondefinition/)() | The default constructor. |
## Methods
| Name | Description |
| --- | --- |
| virtual [GetArrayModeParameters](../../aspose.cells/customfunctiondefinition/getarraymodeparameters/)(string) | Gets the indices of given custom function's parameters that need to be calculated in array mode. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class CustomFunctionDefinitionDemo
{
public static void CustomFunctionDefinitionExample()
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
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
