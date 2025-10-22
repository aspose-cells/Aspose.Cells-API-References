##Enum MsoArrowheadStyle
Aspose.Cells.Drawing.MsoArrowheadStyle enum. Enumerates the line end type of the shape border line
## MsoArrowheadStyle enumeration
Enumerates the line end type of the shape border line.
```csharp
public enum MsoArrowheadStyle
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No line end type. |
| Arrow | `1` | Arrow line end type. |
| ArrowStealth | `2` | Arrow Stealth line end type. |
| ArrowDiamond | `3` | Arrow Diamond Line end type. |
| ArrowOval | `4` | Arrow Oval line end type. |
| ArrowOpen | `5` | Arrow Open line end type. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class DrawingClassMsoArrowheadStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);
// Set line properties
MsoLineFormat lineFormat = lineShape.LineFormat;
lineFormat.ForeColor = System.Drawing.Color.Black;
lineFormat.DashStyle = MsoLineDashStyle.DashDot;
lineFormat.Weight = 0.75;
// Set arrowhead styles
lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;
// Save the workbook
workbook.Save("MsoArrowheadStyleDemo.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
