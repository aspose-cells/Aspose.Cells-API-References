##Workbook.CustomTheme
Workbook method. Customs the theme
## Workbook.CustomTheme method
Customs the theme.
```csharp
public void CustomTheme(string themeName, Color[] colors)
```
| Parameter | Type | Description |
| --- | --- | --- |
| themeName | String | The theme name |
| colors | Color[] | The theme colors |
### Remarks
The length of colors should be 12.
| **Array index** | **Theme type** |
| --- | --- |
| 0 | Backgournd1 |
| 1 | Text1 |
| 2 | Backgournd2 |
| 3 | Text2 |
| 4 | Accent1 |
| 5 | Accent2 |
| 6 | Accent3 |
| 7 | Accent4 |
| 8 | Accent5 |
| 9 | Accent6 |
| 10 | Hyperlink |
| 11 | Followed Hyperlink |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System.Drawing;
public class WorkbookMethodCustomThemeWithStringColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data to demonstrate theme effects
var cell = worksheet.Cells["A1"];
cell.PutValue("Theme Demonstration");
var style = cell.GetStyle();
style.Font.IsBold = true;
style.Font.Size = 14;
cell.SetStyle(style);
// Prepare theme colors
Color[] customColors = new Color[]
{
Color.FromArgb(255, 0, 0),     // Red
Color.FromArgb(0, 255, 0),     // Green
Color.FromArgb(0, 0, 255),     // Blue
Color.FromArgb(255, 255, 0),    // Yellow
Color.FromArgb(255, 0, 255),    // Magenta
Color.FromArgb(0, 255, 255),    // Cyan
Color.FromArgb(128, 0, 128),    // Purple
Color.FromArgb(128, 128, 0),   // Olive
Color.FromArgb(0, 128, 128),    // Teal
Color.FromArgb(128, 0, 0),      // Maroon
Color.FromArgb(0, 128, 0),     // Green (dark)
Color.FromArgb(0, 0, 128)       // Navy
};
try
{
// Apply custom theme
workbook.CustomTheme("MyCustomTheme", customColors);
// Create a styled cell to demonstrate theme effect
var themedCell = worksheet.Cells["A3"];
themedCell.PutValue("Themed Text");
var themedStyle = workbook.CreateStyle();
themedStyle.Font.ThemeColor = new ThemeColor(ThemeColorType.Accent1, 0.0);
themedStyle.Font.Size = 12;
themedCell.SetStyle(themedStyle);
// Save the workbook
workbook.Save("CustomThemeDemo.xlsx");
}
catch (System.Exception ex)
{
System.Console.WriteLine($"Error applying custom theme: {ex.Message}");
}
}
}
}
```
### See Also
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
