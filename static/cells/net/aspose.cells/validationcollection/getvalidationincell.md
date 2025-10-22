##ValidationCollection.GetValidationInCell
ValidationCollection method. Gets the validation applied to given cell
## ValidationCollection.GetValidationInCell method
Gets the validation applied to given cell.
```csharp
public Validation GetValidationInCell(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Return Value
Returns a [`Validation`](../../validation/) object or null if there is no validation for given cell
### Examples
```csharp
using System;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationCollectionMethodGetValidationInCellWithInt32Int32Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data validation to cell A1 (0,0)
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.List;
validation.Formula1 = "\"Option1,Option2,Option3\"";
// Create CellArea with StartRow, StartColumn, EndRow, EndColumn
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
validation.AddArea(area);
// Get validation from cell A1 (0,0)
Validation validationInCell = worksheet.Validations.GetValidationInCell(0, 0);
if (validationInCell != null && validationInCell.Type == ValidationType.List)
{
Console.WriteLine("Cell A1 has list validation with formula: " + validationInCell.Formula1);
}
}
}
}
```
### See Also
* class [Validation](../../validation/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
