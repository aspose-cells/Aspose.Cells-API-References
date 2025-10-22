##Validation.ErrorMessage
Validation property. Represents the data validation error message
## Validation.ErrorMessage property
Represents the data validation error message.
```csharp
public string ErrorMessage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyErrorMessageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create validation for cell A1
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "20";
// Set error message properties
validation.ErrorMessage = "Value must be between 10 and 20";
validation.ErrorTitle = "Invalid Input";
validation.AlertStyle = ValidationAlertType.Stop;
// Apply validation and test it
worksheet.Cells["A1"].PutValue(5); // Invalid value
Console.WriteLine("Validation Error Message: " + validation.ErrorMessage);
// Save the workbook
workbook.Save("ValidationErrorMessageDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
