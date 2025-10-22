##Row.SetStyle
Row method. Sets the style of this row
## Row.SetStyle method
Sets the style of this row.
```csharp
public void SetStyle(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this row. |
### Remarks
This method only sets the given style as the default style for this row, without changing the style settings for existing cells in this row. To update style settings of existing cells to the specified style at the same time, please use [`ApplyStyle`](../applystyle/)
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RowMethodSetStyleWithStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create and configure a style
Style style = workbook.CreateStyle();
style.BackgroundColor = System.Drawing.Color.Blue;
style.ForegroundColor = System.Drawing.Color.Red;
style.Pattern = BackgroundType.DiagonalStripe;
// Get the first row and apply style
Row row = worksheet.Cells.Rows[0];
row.SetStyle(style);
// Save the workbook
workbook.Save("RowStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
