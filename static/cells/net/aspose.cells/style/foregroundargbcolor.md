##Style.ForegroundArgbColor
Style property. Gets and sets the foreground color with a 32bit ARGB value
## Style.ForegroundArgbColor property
Gets and sets the foreground color with a 32-bit ARGB value.
```csharp
public int ForegroundArgbColor { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyForegroundArgbColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with specific foreground color
Style style = workbook.CreateStyle();
style.ForegroundColor = System.Drawing.Color.FromArgb(255, 0, 255, 0); // Green color
style.Pattern = BackgroundType.Solid;
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
// Get and display the foreground ARGB color value
int foregroundArgb = cell.GetStyle().ForegroundArgbColor;
Console.WriteLine("Foreground ARGB Color: " + foregroundArgb);
// Save the workbook
workbook.Save("ForegroundColorDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
