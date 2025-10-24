##Validation.InCellDropDown
Validation property. Indicates whether data validation displays a dropdown list that contains acceptable values
## Validation.InCellDropDown property
Indicates whether data validation displays a drop-down list that contains acceptable values.
```csharp
public bool InCellDropDown { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyInCellDropDownDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation for cell A1
Validation validation = worksheet.Cells["A1"].GetValidation();
// Set validation type to list with values
validation.Type = ValidationType.List;
validation.Formula1 = "Option1,Option2,Option3";
// Enable in-cell dropdown
validation.InCellDropDown = true;
// Create another validation for cell B1 without dropdown
Validation validation2 = worksheet.Cells["B1"].GetValidation();
validation2.Type = ValidationType.List;
validation2.Formula1 = "Choice1,Choice2,Choice3";
validation2.InCellDropDown = false;
// Save the workbook
workbook.Save("InCellDropDownDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
