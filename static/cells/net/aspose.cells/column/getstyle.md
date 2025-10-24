##Column.GetStyle
Column method. Gets the style of this column
## Column.GetStyle method
Gets the style of this column.
```csharp
public Style GetStyle()
```
### Remarks
Modifying the returned style object directly takes no effect for this column or any cells in this column. You have to call [`ApplyStyle`](../applystyle/) or [`SetStyle`](../setstyle/) method to apply the change to this column. Column's style is the style which will be inherited by cells in this column(those cells that have no custom style settings, such as existing cells that have not been set style explicitly, or those that have not been instantiated)
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ColumnMethodGetStyleDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Set style for column 5
Style columnStyle = cells.Columns[5].GetStyle();
columnStyle.Font.Name = "Arial";
columnStyle.Font.Size = 14;
columnStyle.Font.IsBold = true;
cells.Columns[5].ApplyStyle(columnStyle, new StyleFlag { Font = true });
// Set style for row 7
Style rowStyle = cells.Rows[7].GetStyle();
rowStyle.Font.Color = System.Drawing.Color.Red;
rowStyle.Font.IsItalic = true;
cells.Rows[7].ApplyStyle(rowStyle, new StyleFlag { Font = true });
// Verify column style
Style retrievedColumnStyle = cells.Columns[5].GetStyle();
Console.WriteLine("Column 5 Style:");
Console.WriteLine($"Font: {retrievedColumnStyle.Font.Name}, Size: {retrievedColumnStyle.Font.Size}, Bold: {retrievedColumnStyle.Font.IsBold}");
// Verify row style
Style retrievedRowStyle = cells.Rows[7].GetStyle();
Console.WriteLine("\nRow 7 Style:");
Console.WriteLine($"Color: {retrievedRowStyle.Font.Color}, Italic: {retrievedRowStyle.Font.IsItalic}");
// Save the workbook
workbook.Save("ColumnMethodGetStyleDemo_output.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
