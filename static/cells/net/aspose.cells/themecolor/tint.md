##ThemeColor.Tint
ThemeColor property. Gets and sets the tint value
## ThemeColor.Tint property
Gets and sets the tint value.
```csharp
public double Tint { get; set; }
```
### Remarks
The tint value is stored as a double from -1.0 .. 1.0, where -1.0 means 100% darken and 1.0 means 100% lighten. Also, 0.0 means no change.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ThemeColorPropertyTintDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a style with theme color and tint
Style style = workbook.CreateStyle();
style.BackgroundThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.5); // 0.5 tint
// Apply the style to a cell
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
// Get the tint value from the cell's style
double tintValue = cell.GetStyle().BackgroundThemeColor.Tint;
Console.WriteLine("Tint value: " + tintValue);
// Modify the tint value
ThemeColor themeColor = cell.GetStyle().BackgroundThemeColor;
themeColor.Tint = 0.8; // Change tint to 0.8
cell.SetStyle(style);
// Verify the new tint value
Console.WriteLine("Modified tint value: " + cell.GetStyle().BackgroundThemeColor.Tint);
}
}
}
```
### See Also
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
