##Style.ForegroundColor
Style property. Gets or sets a styles foreground color
## Style.ForegroundColor property
Gets or sets a style's foreground color.
```csharp
public Color ForegroundColor { get; set; }
```
### Remarks
It means no color setting if Color.Empty is returned.
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class StylePropertyForegroundColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Style style = workbook.CreateStyle();
style.ForegroundColor = Color.Green;
style.Pattern = BackgroundType.Solid;
Cell cell = worksheet.Cells["A1"];
cell.SetStyle(style);
Console.WriteLine("ForegroundColor set to: " + style.ForegroundColor);
workbook.Save("ForegroundColorDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
