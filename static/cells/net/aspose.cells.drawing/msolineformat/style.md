##MsoLineFormat.Style
MsoLineFormat property. Returns a Style object that represents the style of the specified range
## MsoLineFormat.Style property
Returns a Style object that represents the style of the specified range.
```csharp
public MsoLineStyle Style { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a line shape
Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);
// Get the line format
MsoLineFormat lineFormat = line.LineFormat;
// Set line style properties
lineFormat.Style = MsoLineStyle.ThickBetweenThin;
lineFormat.ForeColor = System.Drawing.Color.Red;
lineFormat.BackColor = System.Drawing.Color.White;
lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
lineFormat.Transparency = 0.5;
lineFormat.Weight = 3.0;
// Create another line for comparison
Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
MsoLineFormat lineFormat2 = line2.LineFormat;
// Copy style from first line to second line
lineFormat2.Style = lineFormat.Style;
lineFormat2.ForeColor = lineFormat.ForeColor;
lineFormat2.BackColor = lineFormat.BackColor;
lineFormat2.DashStyle = lineFormat.DashStyle;
lineFormat2.Transparency = lineFormat.Transparency;
lineFormat2.Weight = lineFormat.Weight;
// Save the workbook
workbook.Save("MsoLineFormatStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
