##Cell.GetValidationValue
Cell method. Gets the value of validation which applied to this cell
## Cell.GetValidationValue method
Gets the value of validation which applied to this cell.
```csharp
public bool GetValidationValue()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetValidationValueDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation range
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.TextLength;
validation.Operator = OperatorType.Between;
validation.Formula1 = "1";
validation.Formula2 = "5";
// Apply validation to cell A1
Cell cell = worksheet.Cells["A1"];
validation.AddArea(new CellArea { StartRow = cell.Row, StartColumn = cell.Column, EndRow = cell.Row, EndColumn = cell.Column });
// Test valid values
string[] validValues = { "a", " ab", "cd ", " xyz " };
foreach (string value in validValues)
{
cell.PutValue(value);
Console.WriteLine($"Value: '{value}' - Valid: {cell.GetValidationValue()}");
}
// Test invalid value
string invalidValue = "toolong";
cell.PutValue(invalidValue);
Console.WriteLine($"Value: '{invalidValue}' - Valid: {cell.GetValidationValue()}");
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
