##ThreeDFormat.Z
ThreeDFormat property. Defines the distance from ground for the 3D shape
## ThreeDFormat.Z property
Defines the distance from ground for the 3D shape.
```csharp
public double Z { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyZDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 100);
// Access the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current Z value (distance from ground)
Console.WriteLine("Current Z value: " + threeDFormat.Z);
// Set new Z value to move the shape further from ground
threeDFormat.Z = 20;
Console.WriteLine("New Z value: " + threeDFormat.Z);
// Configure other 3D properties to make the effect visible
threeDFormat.ExtrusionHeight = 30;
threeDFormat.ContourWidth = 2;
threeDFormat.PresetCameraType = PresetCameraType.PerspectiveContrastingRightFacing;
// Save the workbook to see the 3D effect
workbook.Save("ThreeDFormatPropertyZDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
