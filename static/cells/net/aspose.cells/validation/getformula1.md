##Validation.GetFormula1
Validation method. Gets the value or expression associated with this validation
## GetFormula1(bool, bool) {#getformula1}
Gets the value or expression associated with this validation.
```csharp
public string GetFormula1(bool isR1C1, bool isLocal)
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
public class ValidationMethodGetFormula1WithBooleanBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a validation to the first cell
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "20";
// Apply validation to cell A1
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
validation.AddArea(area);
try
{
// Call GetFormula1 with parameters (false, false) to get the formula in A1 notation
string formula1 = validation.GetFormula1(false, false);
Console.WriteLine("Formula1 in A1 notation: " + formula1);
// Call GetFormula1 with parameters (true, false) to get the formula in R1C1 notation
string formula1R1C1 = validation.GetFormula1(true, false);
Console.WriteLine("Formula1 in R1C1 notation: " + formula1R1C1);
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFormula1 method: {ex.Message}");
}
// Save the workbook
workbook.Save("ValidationMethodGetFormula1WithBooleanBooleanDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## GetFormula1(bool, bool, int, int) {#getformula1_1}
Gets the value or expression associated with this validation for specific cell.
```csharp
public string GetFormula1(bool isR1C1, bool isLocal, int row, int column)
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
public class ValidationMethodGetFormula1WithBooleanBooleanInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create validation in cell B5 (row 4, column 1)
CellArea area = CellArea.CreateCellArea(4, 1, 4, 1); // Use static method via type name
int validationIndex = worksheet.Validations.Add(area); // Get validation index
Validation validation = worksheet.Validations[validationIndex]; // Retrieve validation object
validation.Type = ValidationType.Custom;
validation.Formula1 = "=A5"; // Relative reference to cell A5
try
{
// Call GetFormula1 with R1C1 format for cell B5
string formulaR1C1 = validation.GetFormula1(true, false, 4, 1);
Console.WriteLine($"R1C1 Formula: {formulaR1C1}");
// Call GetFormula1 with A1 format for cell B5
string formulaA1 = validation.GetFormula1(false, false, 4, 1);
Console.WriteLine($"A1 Formula: {formulaA1}");
workbook.Save("ValidationGetFormula1Demo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
