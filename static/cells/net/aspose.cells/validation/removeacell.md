##Validation.RemoveACell
Validation method. Remove the validation settings in the cell
## Validation.RemoveACell method
Remove the validation settings in the cell.
```csharp
public void RemoveACell(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index. |
| column | Int32 | The column index. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodRemoveACellWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data validation to first cell
Validation validation = worksheet.Validations[0];
validation.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 0, EndColumn = 0 });
validation.Type = ValidationType.List;
validation.Formula1 = "1,2,3";
// Add another cell to the validation
validation.AddArea(new CellArea { StartRow = 1, StartColumn = 1, EndRow = 1, EndColumn = 1 });
// Remove the second cell from validation
validation.RemoveACell(1, 1);
Console.WriteLine("Cell removed from validation successfully.");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
