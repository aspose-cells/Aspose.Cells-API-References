##CellsColor.Transparency
CellsColor property. Gets and sets transparency as a value from 0.0 opaque through 1.0 clear
## CellsColor.Transparency property
Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class CellsColorPropertyTransparencyDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
CellsColor cellsColor = workbook.CreateCellsColor();
cellsColor.Color = Color.FromArgb(128, 255, 0, 0); // Semi-transparent red
cellsColor.Transparency = 0.5; // Set transparency to 50%
Style style = workbook.CreateStyle();
style.ForegroundColor = cellsColor.Color;
style.Pattern = BackgroundType.Solid;
worksheet.Cells["A1"].PutValue("50% transparent red background");
worksheet.Cells["A1"].SetStyle(style);
workbook.Save("TransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [CellsColor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
