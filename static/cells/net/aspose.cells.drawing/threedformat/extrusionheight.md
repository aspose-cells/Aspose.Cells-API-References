##ThreeDFormat.ExtrusionHeight
ThreeDFormat property. Gets and sets the extrusion height of the applied to the shape in unit of points
## ThreeDFormat.ExtrusionHeight property
Gets and sets the extrusion height of the applied to the shape, in unit of points.
```csharp
public double ExtrusionHeight { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyExtrusionHeightDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 100, 200, 50);
// Apply 3D formatting
ThreeDFormat threeDFormat = shape.ThreeDFormat;
threeDFormat.ExtrusionHeight = 32;
threeDFormat.ContourWidth = 17;
threeDFormat.TopBevelType = BevelType.HardEdge;
threeDFormat.TopBevelWidth = 30;
threeDFormat.TopBevelHeight = 30;
// Save the workbook
workbook.Save("output.xlsx");
// Verify the saved values
Workbook loadedWorkbook = new Workbook("output.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;
Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
