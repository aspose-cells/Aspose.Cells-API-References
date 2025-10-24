##StyleFlag.LeftBorder
StyleFlag property. Left border settings will be applied
## StyleFlag.LeftBorder property
Left border settings will be applied.
```csharp
public bool LeftBorder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StyleFlagPropertyLeftBorderDemo
{
public static void Run()
{
// Create a workbook
var workbook = new Workbook();
var worksheet = workbook.Worksheets[0];
// Create a range and apply left border style
var range = worksheet.Cells.CreateRange(1, 1, 1, 1);
range.PutValue("Left Border Demo", false, false);
// Create style and flag
var style = workbook.CreateStyle();
var flag = new StyleFlag();
// Set left border properties
style.Borders[BorderType.LeftBorder].Color = Color.Green;
style.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thick;
flag.LeftBorder = true;
// Apply the style with left border flag
range.ApplyStyle(style, flag);
// Verify the left border was applied
var appliedStyle = worksheet.Cells[1, 1].GetStyle();
Console.WriteLine($"Left border color: {appliedStyle.Borders[BorderType.LeftBorder].Color}");
Console.WriteLine($"Left border style: {appliedStyle.Borders[BorderType.LeftBorder].LineStyle}");
// Save the workbook
workbook.Save("LeftBorderDemo.xlsx");
}
}
}
```
### See Also
* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
