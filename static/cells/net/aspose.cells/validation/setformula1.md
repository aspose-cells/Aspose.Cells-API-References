##Validation.SetFormula1
Validation method. Sets the value or expression associated with this validation
## Validation.SetFormula1 method
Sets the value or expression associated with this validation.
```csharp
public void SetFormula1(string formula, bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The value or expression associated with this format condition. |
| isR1C1 | Boolean | Whether the formula is R1C1 formula. |
| isLocal | Boolean | Whether the formula is locale formatted. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationMethodSetFormula1WithStringBooleanBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare sample data in cell B1
worksheet.Cells["B1"].PutValue(100);
// Create data validation for cell A1
int validationIndex = worksheet.Validations.Add(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
Validation validation = worksheet.Validations[validationIndex];
validation.Type = ValidationType.Decimal;
validation.Operator = OperatorType.GreaterOrEqual;
validation.ShowError = true;
validation.ErrorTitle = "Validation Error";
validation.ErrorMessage = "Value must be greater than or equal to cell B1 (100)";
try
{
// Set formula referencing B1 using A1 notation (non-R1C1, non-local)
validation.SetFormula1("=B1", false, false);
Console.WriteLine("SetFormula1 executed successfully with parameters (String, Boolean, Boolean)");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFormula1: {ex.Message}");
}
// Save the workbook with validation
workbook.Save("ValidationSetFormula1Demo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
