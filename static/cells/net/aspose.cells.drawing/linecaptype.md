##Enum LineCapType
Aspose.Cells.Drawing.LineCapType enum. Represents the caps of a line
## LineCapType enumeration
Represents the caps of a line
```csharp
public enum LineCapType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Square | `0` | Square protrudes by half line width. |
| Round | `1` | Rounded ends. |
| Flat | `2` | Line ends at end point. |
| None | `3` | None cap |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassLineCapTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
LineFormat lineFmt = shape.Line;
lineFmt.CapType = LineCapType.Flat;
lineFmt.Weight = 2.0;
lineFmt.DashStyle = MsoLineDashStyle.Solid;
workbook.Save("LineCapTypeDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
