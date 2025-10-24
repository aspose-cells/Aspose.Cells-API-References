##Validation.ShowInput
Validation property. Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range
## Validation.ShowInput property
Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.
```csharp
public bool ShowInput { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyShowInputDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation area
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 0;
area.StartColumn = 0;
area.EndColumn = 0;
// Add validation
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.List;
validation.Formula1 = "Yes,No";
validation.IgnoreBlank = true;
validation.InCellDropDown = true;
// Set ShowInput property
validation.ShowInput = true;
validation.InputTitle = "Selection";
validation.InputMessage = "Please select Yes or No";
validation.AddArea(area);
// Save the workbook
workbook.Save("ValidationPropertyShowInputDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
