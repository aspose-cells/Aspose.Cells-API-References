##ThreeDFormat.ContourWidth
ThreeDFormat property. Gets and sets the contour width on the shape in unit of points
## ThreeDFormat.ContourWidth property
Gets and sets the contour width on the shape, in unit of points.
```csharp
public double ContourWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyContourWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add a shape to the worksheet with all required parameters
Shape sh = ws.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
// Apply 3D formatting
ThreeDFormat n3df = sh.ThreeDFormat;
n3df.ContourWidth = 17;
n3df.ExtrusionHeight = 32;
n3df.TopBevelType = (BevelType)BevelPresetType.HardEdge;
// Save the workbook
wb.Save("output.xlsx");
// Verify the saved values
Workbook wb2 = new Workbook("output.xlsx");
Shape sh2 = wb2.Worksheets[0].Shapes[0];
ThreeDFormat n3df2 = sh2.ThreeDFormat;
Console.WriteLine("ContourWidth: " + n3df2.ContourWidth);
Console.WriteLine("ExtrusionHeight: " + n3df2.ExtrusionHeight);
Console.WriteLine("TopBevelType: " + n3df2.TopBevelType);
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
