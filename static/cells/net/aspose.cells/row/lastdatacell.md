##Row.LastDataCell
Row property. Gets the last nonblank cell in the row
## Row.LastDataCell property
Gets the last non-blank cell in the row.
```csharp
public Cell LastDataCell { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyLastDataCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Put data in cells
cells["A1"].PutValue("First cell");
cells["B1"].PutValue("Second cell");
cells["C2"].PutValue("Not in first row");
// Get last data cell in first row
Cell lastDataCell = cells.Rows[0].LastDataCell;
Console.WriteLine("Last data cell in first row: " + lastDataCell.Name);
Console.WriteLine("Value in last data cell: " + lastDataCell.StringValue);
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
