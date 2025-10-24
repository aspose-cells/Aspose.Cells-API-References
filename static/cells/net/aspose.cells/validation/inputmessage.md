##Validation.InputMessage
Validation property. Represents the data validation input message
## Validation.InputMessage property
Represents the data validation input message.
```csharp
public string InputMessage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyInputMessageDemo
{
public static void Run()
{
// Create workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create validation
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.List;
validation.Formula1 = "Yes,No";
validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
validation.IgnoreBlank = true;
validation.InCellDropDown = true;
// Set input message properties
validation.ShowInput = true;
validation.InputTitle = "Selection Required";
validation.InputMessage = "Please select either Yes or No from the dropdown";
// Save the workbook
workbook.Save("ValidationInputMessageDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
