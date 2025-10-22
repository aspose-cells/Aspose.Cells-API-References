##ThreeDFormat.LightAngle
ThreeDFormat property. Gets and sets the angle of the extrusion lights
## ThreeDFormat.LightAngle property
Gets and sets the angle of the extrusion lights.
```csharp
public double LightAngle { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyLightAngleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 200, 100, 0, 0);
shape.Text = "3D Format Demo";
// Access the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current LightAngle value
Console.WriteLine("Current LightAngle value: " + threeDFormat.LightAngle);
// Set new LightAngle value (0 to 359.9 degrees)
threeDFormat.LightAngle = 45;
Console.WriteLine("New LightAngle value: " + threeDFormat.LightAngle);
// Configure other 3D properties to see the effect of LightAngle
threeDFormat.TopBevelType = BevelType.ArtDeco;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
threeDFormat.Material = PresetMaterialType.Plastic;
threeDFormat.Lighting = LightRigType.ThreePoint;
threeDFormat.LightingDirection = LightRigDirectionType.Top;
// Save the workbook to see the effects
workbook.Save("ThreeDFormatLightAngleDemo.xlsx");
}
}
}
```
### See Also
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
