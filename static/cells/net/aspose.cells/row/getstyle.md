##Row.GetStyle
Row method. Gets the style of this row
## Row.GetStyle method
Gets the style of this row.
```csharp
public Style GetStyle()
```
### Remarks
Modifying the returned style object directly takes no effect for this row or any cells in this row. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this row. Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class RowMethodGetStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set styles for demonstration
Style rowStyle = workbook.CreateStyle();
rowStyle.Pattern = BackgroundType.Solid;
rowStyle.ForegroundColor = System.Drawing.Color.Blue;
cells.Rows[8].ApplyStyle(rowStyle, new StyleFlag { All = true });
Style columnStyle = workbook.CreateStyle();
columnStyle.Pattern = BackgroundType.Solid;
columnStyle.ForegroundColor = System.Drawing.Color.Red;
cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { All = true });
// Demonstrate GetStyle usage
Style retrievedRowStyle = cells.Rows[8].GetStyle();
Console.WriteLine("Row 8 Style - ForegroundColor: " + retrievedRowStyle.ForegroundColor);
Console.WriteLine("Row 8 Style - Pattern: " + retrievedRowStyle.Pattern);
Style retrievedColumnStyle = cells.Columns[5].GetStyle();
Console.WriteLine("Column 5 Style - ForegroundColor: " + retrievedColumnStyle.ForegroundColor);
Console.WriteLine("Column 5 Style - Pattern: " + retrievedColumnStyle.Pattern);
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Row](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
