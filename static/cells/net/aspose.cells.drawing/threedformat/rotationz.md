##ThreeDFormat.RotationZ
ThreeDFormat property. Gets and sets the rotation of the extruded shape around the zaxis in degrees
## ThreeDFormat.RotationZ property
Gets and sets the rotation of the extruded shape around the z-axis in degrees.
```csharp
public double RotationZ { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyRotationZDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 2, 0, 2, 0, 100, 150);
shape.Text = "3D Rotation Demo";
// Access the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current RotationZ value
Console.WriteLine("Current RotationZ value: " + threeDFormat.RotationZ);
// Set new RotationZ values and demonstrate effects
threeDFormat.RotationZ = 45;
Console.WriteLine("Shape rotated 45 degrees around Z-axis");
// Apply other 3D properties to make rotation visible
threeDFormat.ExtrusionHeight = 15;
threeDFormat.ContourWidth = 2;
threeDFormat.PresetCameraType = PresetCameraType.OrthographicFront;
// Save the workbook with the 3D effects
workbook.Save("ThreeDFormatRotationZDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
