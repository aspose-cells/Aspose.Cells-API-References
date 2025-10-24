##ThemeColor.ThemeColor
ThemeColor constructor.
## ThemeColor constructor
```csharp
public ThemeColor(ThemeColorType type, double tint)
```
| Parameter | Type | Description |
| --- | --- | --- |
| type | ThemeColorType | The theme type. |
| tint | Double | The tint value. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ThemeColorMethodCtorWithThemeColorTypeDoubleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Call the #ctor method with ThemeColorType and Double parameters
ThemeColor themeColor = new ThemeColor(ThemeColorType.Accent1, 0.5);
// Apply the theme color to a cell's style
Style style = workbook.CreateStyle();
style.ForegroundThemeColor = themeColor;
style.Pattern = BackgroundType.Solid;
Cell cell = worksheet.Cells["A1"];
cell.PutValue("ThemeColor with Accent1 and 0.5 tint");
cell.SetStyle(style);
Console.WriteLine("ThemeColor constructor executed successfully with parameters (ThemeColorType.Accent1, 0.5)");
Console.WriteLine($"ColorType: {themeColor.ColorType}, Tint: {themeColor.Tint}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing ThemeColor constructor: {ex.Message}");
}
// Save the result
workbook.Save("ThemeColorCtorDemo.xlsx");
}
}
}
```
### See Also
* enum [ThemeColorType](../../themecolortype/)
* class [ThemeColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
