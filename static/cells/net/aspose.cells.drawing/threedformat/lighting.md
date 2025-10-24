##ThreeDFormat.Lighting
ThreeDFormat property. Gets and sets type of light rig
## ThreeDFormat.Lighting property
Gets and sets type of light rig.
```csharp
public LightRigType Lighting { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyLightingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 200);
shape.Text = "3D Lighting Demo";
// Get the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current lighting value
Console.WriteLine("Current Lighting value: " + threeDFormat.Lighting);
// Set different lighting types and observe effects
threeDFormat.Lighting = LightRigType.BrightRoom;
Console.WriteLine("Changed to BrightRoom lighting");
// Apply some other 3D properties to better see the lighting effect
threeDFormat.TopBevelType = BevelType.ArtDeco;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
// Save with first lighting type
workbook.Save("BrightRoomLighting.xlsx");
// Change to another lighting type
threeDFormat.Lighting = LightRigType.Sunset;
Console.WriteLine("Changed to Sunset lighting");
workbook.Save("SunsetLighting.xlsx");
// Change to a third lighting type
threeDFormat.Lighting = LightRigType.ThreePoint;
Console.WriteLine("Changed to ThreePoint lighting");
workbook.Save("ThreePointLighting.xlsx");
}
}
}
```
### See Also
* enum [LightRigType](../../lightrigtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
