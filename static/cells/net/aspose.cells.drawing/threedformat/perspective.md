##ThreeDFormat.Perspective
ThreeDFormat property. Gets and sets the angle at which a ThreeDFormat object can be viewed
## ThreeDFormat.Perspective property
Gets and sets the angle at which a ThreeDFormat object can be viewed.
```csharp
public double Perspective { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyPerspectiveDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 0, 0, 0, 0, 200, 100);
// Get the 3D format of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current perspective value
Console.WriteLine("Current Perspective value: " + threeDFormat.Perspective);
// Set new perspective value (0 to 120 degrees)
threeDFormat.Perspective = 45;
Console.WriteLine("Perspective set to: " + threeDFormat.Perspective);
// Apply other 3D effects to better visualize the perspective change
threeDFormat.ExtrusionHeight = 15;
threeDFormat.ContourWidth = 2;
threeDFormat.RotationX = 20;
threeDFormat.RotationY = 30;
// Save the workbook to see the effects
workbook.Save("ThreeDFormatPerspectiveDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
