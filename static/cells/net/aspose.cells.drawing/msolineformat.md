##Class MsoLineFormat
Aspose.Cells.Drawing.MsoLineFormat class. Represents line and arrowhead formatting
## MsoLineFormat class
Represents line and arrowhead formatting.
```csharp
public class MsoLineFormat
```
## Properties
| Name | Description |
| --- | --- |
| [BackColor](../../aspose.cells.drawing/msolineformat/backcolor/) { get; set; } | Gets and sets the border line back color. |
| [DashStyle](../../aspose.cells.drawing/msolineformat/dashstyle/) { get; set; } | Gets or sets the dash style for the specified line. |
| [ForeColor](../../aspose.cells.drawing/msolineformat/forecolor/) { get; set; } | Gets and sets the border line fore color. |
| [IsVisible](../../aspose.cells.drawing/msolineformat/isvisible/) { get; set; } | Indicates whether the object is visible. |
| [Style](../../aspose.cells.drawing/msolineformat/style/) { get; set; } | Returns a Style object that represents the style of the specified range. |
| [Transparency](../../aspose.cells.drawing/msolineformat/transparency/) { get; set; } | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [Weight](../../aspose.cells.drawing/msolineformat/weight/) { get; set; } | Returns or sets the weight of the line ,in units of pt. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class MsoLineFormatDemo
{
public static void MsoLineFormatExample()
{
// Instantiate a new Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape to the worksheet
Aspose.Cells.Drawing.ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);
// Get the MsoLineFormat object from the shape
MsoLineFormat lineFormat = arcShape.LineFormat;
// Set properties of the MsoLineFormat object
lineFormat.IsVisible = true;
lineFormat.Style = MsoLineStyle.ThickThin;
lineFormat.ForeColor = Color.Red;
lineFormat.BackColor = Color.Blue;
lineFormat.DashStyle = MsoLineDashStyle.Solid;
lineFormat.Transparency = 0.5;
lineFormat.Weight = 2.0;
// Save the workbook
workbook.Save("MsoLineFormatExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)
