##MsoLineFormat.DashStyle
MsoLineFormat property. Gets or sets the dash style for the specified line
## MsoLineFormat.DashStyle property
Gets or sets the dash style for the specified line.
```csharp
public MsoLineDashStyle DashStyle { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class MsoLineFormatPropertyDashStyleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a shape to demonstrate DashStyle
Shape shape = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 1, 0, 200, 100);
// Set line properties
shape.LineFormat.Style = MsoLineStyle.Single;
shape.LineFormat.Weight = 3;
shape.LineFormat.ForeColor = Color.Blue;
// Demonstrate different dash styles
shape.LineFormat.DashStyle = MsoLineDashStyle.Solid;
shape.Text = "Solid Line";
// Add another shape with different dash style
Shape shape2 = workbook.Worksheets[0].Shapes.AddRectangle(1, 0, 3, 0, 200, 100);
shape2.LineFormat.Style = MsoLineStyle.Single;
shape2.LineFormat.Weight = 3;
shape2.LineFormat.ForeColor = Color.Red;
shape2.LineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
shape2.Text = "DashDotDot Line";
// Save the workbook
workbook.Save("LineDashStyleDemo.xlsx");
}
}
}
```
### See Also
* enum [MsoLineDashStyle](../../msolinedashstyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
