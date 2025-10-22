##ThreeDFormat.TopBevelWidth
ThreeDFormat property. Gets and sets the width of the top bevel or how far into the shape it is applied. In unit of Points
## ThreeDFormat.TopBevelWidth property
Gets and sets the width of the top bevel, or how far into the shape it is applied. In unit of Points.
```csharp
public double TopBevelWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ThreeDFormatPropertyTopBevelWidthDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to the worksheet with correct parameters
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 10, 10, 200, 200, 0, 0);
// Get the 3D format of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Set 3D properties including TopBevelWidth
threeDFormat.TopBevelType = BevelType.HardEdge;
threeDFormat.TopBevelWidth = 30;
threeDFormat.TopBevelHeight = 30;
threeDFormat.ContourWidth = 17;
threeDFormat.ExtrusionHeight = 32;
// Save the workbook
workbook.Save("ThreeDFormatDemo.xlsx");
// Verify the saved properties
Workbook loadedWorkbook = new Workbook("ThreeDFormatDemo.xlsx");
Shape loadedShape = loadedWorkbook.Worksheets[0].Shapes[0];
ThreeDFormat loadedFormat = loadedShape.ThreeDFormat;
Console.WriteLine("TopBevelWidth: " + loadedFormat.TopBevelWidth);
Console.WriteLine("TopBevelHeight: " + loadedFormat.TopBevelHeight);
Console.WriteLine("TopBevelType: " + loadedFormat.TopBevelType);
Console.WriteLine("ContourWidth: " + loadedFormat.ContourWidth);
Console.WriteLine("ExtrusionHeight: " + loadedFormat.ExtrusionHeight);
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
