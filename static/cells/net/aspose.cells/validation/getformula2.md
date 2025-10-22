##Validation.GetFormula2
Validation method. Gets the value or expression associated with this validation
## GetFormula2(bool, bool) {#getformula2}
Gets the value or expression associated with this validation.
```csharp
public string GetFormula2(bool isR1C1, bool isLocal)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
### Return Value
The value or expression associated with this validation.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationMethodGetFormula2WithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a validation to a cell range
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "20";
// Add validation area
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 0;
area.StartColumn = 0;
area.EndColumn = 0;
validation.AddArea(area);
try
{
// Call GetFormula2 with parameters (isR1C1: false, isLocal: false)
string formula2 = validation.GetFormula2(false, false);
Console.WriteLine("Formula2: " + formula2);
Console.WriteLine("Method executed successfully with parameters (Boolean, Boolean)");
// Display the validation settings
Console.WriteLine("Validation Type: " + validation.Type);
Console.WriteLine("Validation Operator: " + validation.Operator);
Console.WriteLine("Validation Formula1: " + validation.Formula1);
Console.WriteLine("Validation Formula2: " + validation.Formula2);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula2 method: {ex.Message}");
}
// Save the workbook
workbook.Save("ValidationMethodGetFormula2Demo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetFormula2(bool, bool, int, int) {#getformula2_1}
Gets the value or expression associated with this validation for specific cell.
```csharp
public string GetFormula2(bool isR1C1, bool isLocal, int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | Boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | Boolean | Whether the formula needs to be formatted by locale. |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
The value or expression associated with this validation.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationMethodGetFormula2WithBooleanBooleanInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create data validation in cell A1
worksheet.Validations.Add();
Validation validation = worksheet.Validations[worksheet.Validations.Count - 1];
validation.Type = ValidationType.Custom;
validation.Operator = OperatorType.Between;
validation.Formula2 = "=B1"; // A1-style formula
validation.AddArea(CellArea.CreateCellArea(0, 0, 0, 0)); // Apply to cell A1 (row 0, column 0)
try
{
// Get Formula2 in R1C1 format for cell A1
string formulaR1C1 = validation.GetFormula2(true, false, 0, 0);
Console.WriteLine($"Formula2 (R1C1 format): {formulaR1C1}");
// Demonstrate original formula remains unchanged
Console.WriteLine($"Original Formula2 (A1 format): {validation.Formula2}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula2: {ex.Message}");
}
workbook.Save("ValidationGetFormula2Demo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
