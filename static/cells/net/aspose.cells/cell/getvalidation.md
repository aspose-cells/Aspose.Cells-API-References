##Cell.GetValidation
Cell method. Gets the validation applied to this cell
## Cell.GetValidation method
Gets the validation applied to this cell.
```csharp
public Validation GetValidation()
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellMethodGetValidationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Access cell B5 and add validation
Cell cell = worksheet.Cells["B5"];
Validation validation = cell.GetValidation();
// Set validation type and show message
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "20";
validation.ShowError = true;
validation.ErrorMessage = "Enter value between 10 and 20";
// Save the workbook
workbook.Save("ValidationDemo.xlsx");
// Verify the validation
Validation retrievedValidation = cell.GetValidation();
Console.WriteLine("Validation Type: " + retrievedValidation.Type);
Console.WriteLine("Validation Message: " + retrievedValidation.ErrorMessage);
}
}
}
```
### See Also
* class [Validation](../../validation/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
