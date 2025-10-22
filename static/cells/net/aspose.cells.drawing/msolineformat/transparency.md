##MsoLineFormat.Transparency
MsoLineFormat property. Returns or sets the degree of transparency of the specified fill as a value from 0.0 opaque through 1.0 clear
## MsoLineFormat.Transparency property
Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an arc shape
ArcShape arc = worksheet.Shapes.AddArc(1, 0, 1, 0, 100, 100);
// Set line format properties including transparency
arc.LineFormat.ForeColor = System.Drawing.Color.Red;
arc.LineFormat.Transparency = 0.5; // 50% transparent
arc.LineFormat.Weight = 3;
arc.LineFormat.DashStyle = MsoLineDashStyle.Solid;
// Create another arc for comparison
ArcShape arc2 = worksheet.Shapes.AddArc(1, 2, 1, 2, 100, 100);
arc2.LineFormat.ForeColor = System.Drawing.Color.Red;
arc2.LineFormat.Transparency = 0.5; // Same transparency
arc2.LineFormat.Weight = 3;
arc2.LineFormat.DashStyle = MsoLineDashStyle.Solid;
// Verify transparency property
if (Math.Abs(arc.LineFormat.Transparency - arc2.LineFormat.Transparency) < 0.001)
{
Console.WriteLine("Transparency properties match: " + arc.LineFormat.Transparency);
}
else
{
Console.WriteLine("Transparency properties do not match");
}
// Save the workbook
workbook.Save("MsoLineFormatTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
