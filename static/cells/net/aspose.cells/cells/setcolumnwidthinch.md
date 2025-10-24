##Cells.SetColumnWidthInch
Cells method. Sets column width in unit of inches in normal view
## Cells.SetColumnWidthInch method
Sets column width in unit of inches in normal view.
```csharp
public void SetColumnWidthInch(int column, double inches)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| inches | Double | Number of inches. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetColumnWidthInchWithInt32DoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set column widths in inches
cells.SetColumnWidthInch(0, 2.0);
cells.SetColumnWidthInch(1, 1.5);
cells.SetColumnWidthInch(2, 0.8);
// Set some data in cells to make the file visible
cells["A1"].PutValue("Column A (2 inches)");
cells["B1"].PutValue("Column B (1.5 inches)");
cells["C1"].PutValue("Column C (0.8 inches)");
// Save the workbook
workbook.Save("ColumnWidthsInInches.xlsx");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
