##Style.BackgroundArgbColor
Style property. Gets and sets the background color with a 32bit ARGB value
## Style.BackgroundArgbColor property
Gets and sets the background color with a 32-bit ARGB value.
```csharp
public int BackgroundArgbColor { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StylePropertyBackgroundArgbColorDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
Style style = cell.GetStyle();
style.BackgroundArgbColor = Color.Yellow.ToArgb();
style.Pattern = BackgroundType.Solid;
cell.SetStyle(style);
cell.PutValue("Sample Text with Yellow Background");
workbook.Save("BackgroundArgbColorDemo.xlsx");
}
}
}
```
### See Also
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
