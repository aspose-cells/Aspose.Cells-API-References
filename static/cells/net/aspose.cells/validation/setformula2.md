##Validation.SetFormula2
Validation method. Sets the value or expression associated with this validation
## Validation.SetFormula2 method
Sets the value or expression associated with this validation.
```csharp
public void SetFormula2(string formula, bool isR1C1, bool isLocal)
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
public class ValidationMethodSetFormula2WithStringBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate sample reference values
worksheet.Cells["A1"].PutValue(100);
worksheet.Cells["B1"].PutValue(200);
// Create data validation for cell C1
ValidationCollection validations = worksheet.Validations;
Validation validation = validations[validations.Add()];
validation.AddArea(CellArea.CreateCellArea(0, 0, 2, 2)); // Applies to cell C1
// Configure validation parameters
validation.Type = ValidationType.Custom;
validation.Operator = OperatorType.Between;
validation.ShowError = true;
validation.ErrorTitle = "Range Error";
validation.ErrorMessage = "Value must be between A1 (100) and B1 (200)";
try
{
// Set validation formulas using required parameter types
validation.SetFormula1("=A1", false, false);
validation.SetFormula2("=B1", false, false); // Demonstrate (String, Boolean, Boolean)
Console.WriteLine("SetFormula2 executed successfully with formula '=B1'");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save the modified workbook
workbook.Save("ValidationSetFormula2Demo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
