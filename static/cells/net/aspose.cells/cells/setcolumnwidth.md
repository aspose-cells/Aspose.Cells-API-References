##Cells.SetColumnWidth
Cells method. Sets the width of the specified column in normal view
## Cells.SetColumnWidth method
Sets the width of the specified column in normal view.
```csharp
public void SetColumnWidth(int column, double width)
```
| Parameter | Type | Description |
| --- | --- | --- |
| column | Int32 | Column index. |
| width | Double | Width of column in unit of characters.Column width must be between 0 and 255. |
### Remarks
For spreadsheet, column width is measured as the number of characters of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodSetColumnWidthWithInt32DoubleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Cells cells = workbook.Worksheets[0].Cells;
cells.SetColumnWidth(0, 25.5);
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
