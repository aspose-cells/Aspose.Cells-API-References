##Validation.Operator
Validation property. Represents the operator for the data validation
## Validation.Operator property
Represents the operator for the data validation.
```csharp
public OperatorType Operator { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyOperatorDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for validation
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue(30);
worksheet.Cells["A4"].PutValue(40);
// Create a validation range
CellArea area = CellArea.CreateCellArea("B1", "B5");
int validationIndex = worksheet.Validations.Add(area);
Validation validation = worksheet.Validations[validationIndex];
// Set validation properties with Operator demonstration
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "30";
validation.ShowError = true;
validation.ErrorMessage = "Value must be between 10 and 30";
// Save the workbook
workbook.Save("ValidationOperatorDemo.xlsx");
}
}
}
```
### See Also
* enum [OperatorType](../../operatortype/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
