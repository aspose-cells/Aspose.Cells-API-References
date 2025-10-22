##Cells.UnhideColumn
Cells method. Unhides a column
## Cells.UnhideColumn method
Unhides a column
```csharp
public void UnhideColumn(int column, double width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| width | Double | Column width. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodUnhideColumnWithInt32DoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
// Hide column 2
cells.HideColumn(2);
// Unhide column 2 with width adjustment (-1 means using standard width)
cells.UnhideColumn(2, -1);
Console.WriteLine("Column 2 width after unhiding: " + cells.Columns[2].Width);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
