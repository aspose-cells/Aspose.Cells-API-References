##Validation.Type
Validation property. Represents the data validation type
## Validation.Type property
Represents the data validation type.
```csharp
public ValidationType Type { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a validation to cell A1
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.ErrorTitle = "Number Validation";
validation.ErrorMessage = "Please enter a whole number";
validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
// Demonstrate the Type property
Console.WriteLine("Validation Type: " + validation.Type);
// Save the workbook
workbook.Save("ValidationExample.xlsx");
}
}
}
```
### See Also
* enum [ValidationType](../../validationtype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
