##Column.SetStyle
Column method. Sets the style of this column
## Column.SetStyle method
Sets the style of this column.
```csharp
public void SetStyle(Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | the style to be used as the default style for cells in this column. |
### Remarks
This method only sets the given style as the default style for this column, without changing the style settings for existing cells in this column. To update style settings of existing cells to the specified style at the same time, please use [`ApplyStyle`](../applystyle/)
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Drawing;
public class ColumnMethodSetStyleDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access the first column
Column column = worksheet.Cells.Columns[0];
// Create a new style from workbook
Style style = workbook.CreateStyle();
style.HorizontalAlignment = TextAlignmentType.Center;
style.VerticalAlignment = TextAlignmentType.Center;
style.Font.Name = "Arial";
style.Font.Size = 12;
style.Font.IsBold = true;
style.ForegroundColor = Color.LightBlue;
style.Pattern = BackgroundType.Solid;
try
{
// Apply the custom style to the entire column
column.SetStyle(style);
Console.WriteLine($"Style applied successfully to column {column.Index}");
Console.WriteLine($"Font: {style.Font.Name}, Size: {style.Font.Size}, Bold: {style.Font.IsBold}");
Console.WriteLine($"Background: {style.ForegroundColor.Name}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetStyle method: {ex.Message}");
}
// Save the modified workbook
workbook.Save("ColumnMethodSetStyleDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../../style/)
* class [Column](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
