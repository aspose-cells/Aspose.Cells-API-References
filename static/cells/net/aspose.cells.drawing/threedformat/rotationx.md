##ThreeDFormat.RotationX
ThreeDFormat property. Gets and sets the rotation of the extruded shape around the xaxis in degrees
## ThreeDFormat.RotationX property
Gets and sets the rotation of the extruded shape around the x-axis in degrees.
```csharp
public double RotationX { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyRotationXDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 2, 2, 2, 200, 100, 100);
// Get 3D format (no need to "enable" 3D effects - just set the properties)
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current RotationX value
Console.WriteLine("Current RotationX value: " + threeDFormat.RotationX);
// Set new RotationX value (rotation around x-axis in degrees)
threeDFormat.RotationX = 45;
Console.WriteLine("New RotationX value: " + threeDFormat.RotationX);
// Set other 3D properties to make the rotation visible
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;
// Save the workbook to see the effects
workbook.Save("ThreeDFormatRotationXDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
