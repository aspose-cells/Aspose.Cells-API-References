##Enum ValidationAlertType
Aspose.Cells.ValidationAlertType enum. Represents the data validation alert style
## ValidationAlertType enumeration
Represents the data validation alert style.
```csharp
public enum ValidationAlertType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Information | `0` | Information alert style. |
| Stop | `1` | Stop alert style. |
| Warning | `2` | Warning alert style. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationAlertTypeDemo
{
public static void ValidationAlertTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Define a cell area for validation
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
// Add a validation to the worksheet
ValidationCollection validations = worksheet.Validations;
int validationIndex = validations.Add(area);
Validation validation = validations[validationIndex];
// Set validation properties
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";
validation.AlertStyle = ValidationAlertType.Stop; // Using the ValidationAlertType enum
validation.ErrorTitle = "Invalid Input";
validation.ErrorMessage = "Please enter a number between 3 and 1234.";
validation.ShowError = true;
// Save the workbook
workbook.Save("ValidationAlertTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
