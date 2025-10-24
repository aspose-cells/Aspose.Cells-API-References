##Worksheet.Validations
Worksheet property. Gets the data validation setting collection in the worksheet
## Worksheet.Validations property
Gets the data validation setting collection in the worksheet.
```csharp
public ValidationCollection Validations { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorksheetPropertyValidationsDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data validation to cell A1
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.List;
validation.Formula1 = "Option1,Option2,Option3";
// Fix: Create CellArea with StartRow, StartColumn, EndRow, EndColumn
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
validation.AddArea(area);
// Get validation from cell A1
Validation cellValidation = worksheet.Validations.GetValidationInCell(0, 0);
// Output validation type
Console.WriteLine("Validation type in A1: " + cellValidation.Type);
// Save the workbook
workbook.Save("ValidationDemo.xlsx");
}
}
}
```
### See Also
* class [ValidationCollection](../../validationcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
