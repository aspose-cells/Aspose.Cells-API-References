##Validation.ShowError
Validation property. Indicates whether the data validation error message will be displayed whenever the user enters invalid data
## Validation.ShowError property
Indicates whether the data validation error message will be displayed whenever the user enters invalid data.
```csharp
public bool ShowError { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyShowErrorDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create validation for cell A1
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
// Set validation properties
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "20";
// Configure error alert
validation.ShowError = true;
validation.ErrorTitle = "Invalid Input";
validation.ErrorMessage = "Value must be between 10 and 20";
// Create another validation to demonstrate property copying
Validation targetValidation = worksheet.Validations[worksheet.Validations.Add()];
targetValidation.AddArea(new CellArea { StartRow = 1, StartColumn = 0, EndRow = 1, EndColumn = 0 });
// Copy ShowError and related properties from first validation
targetValidation.ShowError = validation.ShowError;
targetValidation.ErrorTitle = validation.ErrorTitle;
targetValidation.ErrorMessage = validation.ErrorMessage;
// Save the workbook
workbook.Save("ValidationShowErrorDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
