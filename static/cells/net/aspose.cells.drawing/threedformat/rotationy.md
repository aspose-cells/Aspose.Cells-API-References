##ThreeDFormat.RotationY
ThreeDFormat property. Gets and sets the rotation of the extruded shape around the yaxis in degrees
## ThreeDFormat.RotationY property
Gets and sets the rotation of the extruded shape around the y-axis in degrees.
```csharp
public double RotationY { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyRotationYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 100, 150, 150);
shape.Text = "3D Rotation Demo";
// Access the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current RotationY value
Console.WriteLine("Current RotationY value: " + threeDFormat.RotationY);
// Set new RotationY values and demonstrate effects
threeDFormat.RotationY = 15;
Console.WriteLine("Shape rotated 15 degrees around Y-axis");
// Apply some other 3D properties to make the effect visible
threeDFormat.ExtrusionHeight = 5;
threeDFormat.ContourWidth = 1;
threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;
// Save the workbook to show the effects
workbook.Save("ThreeDFormatRotationYDemo.xlsx");
// Change rotation again and save another version
threeDFormat.RotationY = 45;
workbook.Save("ThreeDFormatRotationYDemo_45degrees.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
