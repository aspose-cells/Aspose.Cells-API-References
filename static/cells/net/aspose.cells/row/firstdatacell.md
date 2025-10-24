##Row.FirstDataCell
Row property. Gets the first nonblank cell in the row
## Row.FirstDataCell property
Gets the first non-blank cell in the row.
```csharp
public Cell FirstDataCell { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowPropertyFirstDataCellDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Put values in different cells
cells["A1"].PutValue("Header");
cells["B2"].PutValue("FirstData");
cells["C2"].PutValue("SecondData");
// Get the first data cell in row 1 (index 0)
Cell firstDataCellRow1 = cells.Rows[0].FirstDataCell;
Console.WriteLine("First data cell in row 1: " + (firstDataCellRow1 != null ? firstDataCellRow1.Name : "null"));
// Get the first data cell in row 2 (index 1)
Cell firstDataCellRow2 = cells.Rows[1].FirstDataCell;
Console.WriteLine("First data cell in row 2: " + firstDataCellRow2.Name);
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
