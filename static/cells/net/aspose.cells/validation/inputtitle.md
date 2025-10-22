##Validation.InputTitle
Validation property. Represents the title of the datavalidation input dialog box
## Validation.InputTitle property
Represents the title of the data-validation input dialog box.
```csharp
public string InputTitle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyInputTitleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation object
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.IgnoreBlank = true;
// Set validation range
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 0;
area.StartColumn = 0;
area.EndColumn = 0;
validation.AddArea(area);
// Set validation properties
validation.Formula1 = "10";
validation.Formula2 = "100";
validation.Operator = OperatorType.Between;
// Set input message properties
validation.InputTitle = "Number Validation";
validation.InputMessage = "Please enter a number between 10 and 100";
// Save the workbook
workbook.Save("ValidationInputTitleDemo.xlsx");
// Verify the InputTitle property
Console.WriteLine("Validation InputTitle: " + validation.InputTitle);
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
