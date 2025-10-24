##Validation.ErrorTitle
Validation property. Represents the title of the datavalidation error dialog box
## Validation.ErrorTitle property
Represents the title of the data-validation error dialog box.
```csharp
public string ErrorTitle { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyErrorTitleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(0, 0, 1, 1))];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "3";
validation.Formula2 = "1234";
validation.ErrorTitle = "Invalid Input";
validation.ErrorMessage = "Value must be between 3 and 1234";
validation.ShowError = true;
workbook.Save("ValidationErrorTitleDemo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
