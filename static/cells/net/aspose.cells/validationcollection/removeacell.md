##ValidationCollection.RemoveACell
ValidationCollection method. Removes all validation setting on the cell
## ValidationCollection.RemoveACell method
Removes all validation setting on the cell.
```csharp
public void RemoveACell(int row, int column)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | The row index of the cell. |
| column | Int32 | The column index of the cell. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationCollectionMethodRemoveACellWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add validation to cell A1 (row 0, column 0)
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
Validation validation = worksheet.Validations[worksheet.Validations.Add(area)];
validation.Type = ValidationType.List;
validation.Formula1 = "Item1,Item2,Item3";
// Remove validation from cell A1
worksheet.Validations.RemoveACell(0, 0);
Console.WriteLine("Validations count after removal: " + worksheet.Validations.Count);
}
}
}
```
### See Also
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
