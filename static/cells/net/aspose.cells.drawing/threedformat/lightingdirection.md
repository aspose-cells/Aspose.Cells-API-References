##ThreeDFormat.LightingDirection
ThreeDFormat property. Gets and sets the direction from which the light rig is oriented in relation to the scene
## ThreeDFormat.LightingDirection property
Gets and sets the direction from which the light rig is oriented in relation to the scene.
```csharp
public LightRigDirectionType LightingDirection { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyLightingDirectionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
shape.Text = "3D Lighting Direction Demo";
// Get the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Set initial 3D properties
threeDFormat.TopBevelType = BevelType.ArtDeco;
threeDFormat.TopBevelWidth = 10;
threeDFormat.TopBevelHeight = 10;
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.Lighting = LightRigType.ThreePoint;
threeDFormat.Material = PresetMaterialType.Plastic;
// Display current lighting direction
Console.WriteLine("Current LightingDirection: " + threeDFormat.LightingDirection);
// Change lighting direction and observe effects
threeDFormat.LightingDirection = LightRigDirectionType.TopLeft;
Console.WriteLine("Changed LightingDirection to TopLeft");
// Change to another direction
threeDFormat.LightingDirection = LightRigDirectionType.BottomRight;
Console.WriteLine("Changed LightingDirection to BottomRight");
// Save the workbook to see the visual effects
workbook.Save("ThreeDFormatLightingDirectionDemo.xlsx");
}
}
}
```
### See Also
* enum [LightRigDirectionType](../../lightrigdirectiontype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
