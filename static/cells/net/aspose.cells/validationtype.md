##Enum ValidationType
Aspose.Cells.ValidationType enum. Represents data validation type
## ValidationType enumeration
Represents data validation type.
```csharp
public enum ValidationType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| AnyValue | `0` | Any value validation type. |
| WholeNumber | `1` | Whole number validation type. |
| Decimal | `2` | Decimal validation type. |
| List | `3` | List validation type. |
| Date | `4` | Date validation type. |
| Time | `5` | Time validation type. |
| TextLength | `6` | Text length validation type. |
| Custom | `7` | Custom validation type. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationTypeDemo
{
public static void ValidationTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a validation to the worksheet
ValidationCollection validations = worksheet.Validations;
CellArea area = CellArea.CreateCellArea(0, 0, 1, 1);
Validation validation = validations[validations.Add(area)];
// Set validation type to WholeNumber
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";
// Set additional properties for the validation
validation.InputMessage = "Please enter a whole number between 3 and 1234.";
validation.InputTitle = "Whole Number Validation";
validation.ErrorMessage = "The value must be a whole number between 3 and 1234.";
validation.ErrorTitle = "Invalid Input";
validation.ShowInput = true;
validation.ShowError = true;
// Save the workbook
workbook.Save("ValidationTypeExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
