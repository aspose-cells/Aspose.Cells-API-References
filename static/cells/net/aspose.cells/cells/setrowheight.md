##Cells.SetRowHeight
Cells method. Sets the height of the specified row
## Cells.SetRowHeight method
Sets the height of the specified row.
```csharp
public void SetRowHeight(int row, double height)
```
| Parameter | Type | Description |
| --- | --- | --- |
| row | Int32 | Row index. |
| height | Double | Height of row.In unit of point It should be between 0 and 409.5. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetRowHeightWithInt32DoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set row height for first row (index 0) to 25.5 points
cells.SetRowHeight(0, 25.5);
// Verify the row height
Console.WriteLine("Row height of row 0: " + cells.GetRowHeight(0));
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
