##Cell.Row
Cell property. Gets row number zero based of the cell
## Cell.Row property
Gets row number (zero based) of the cell.
```csharp
public int Row { get; }
```
### Property Value
Cell row number
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellPropertyRowDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and formula
worksheet.Cells["A1"].PutValue(10);
worksheet.Cells["A2"].PutValue(20);
worksheet.Cells["A3"].PutValue("=SUM(A1:A2)");
// Find cell containing formula
Cell cell = worksheet.Cells.Find("=SUM(A1", null, new FindOptions()
{
LookInType = LookInType.OnlyFormulas,
LookAtType = LookAtType.Contains
});
// Demonstrate Row property
Console.WriteLine("Formula found in row: " + cell.Row);
Console.WriteLine("Formula found in column: " + cell.Column);
// Verify the row is correct
if (cell.Row == 2 && cell.Column == 0)
{
Console.WriteLine("Row property works correctly");
}
}
}
}
```
### See Also
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
