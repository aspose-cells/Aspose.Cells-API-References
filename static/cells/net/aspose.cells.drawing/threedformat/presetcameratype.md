##ThreeDFormat.PresetCameraType
ThreeDFormat property. Gets and sets the extrusion preset camera type
## ThreeDFormat.PresetCameraType property
Gets and sets the extrusion preset camera type.
```csharp
public PresetCameraType PresetCameraType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyPresetCameraTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.Rectangle, 1, 1, 0, 0, 200, 200);
// Get the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display the current PresetCameraType value
Console.WriteLine("Current PresetCameraType: " + threeDFormat.PresetCameraType);
// Set a new PresetCameraType value
threeDFormat.PresetCameraType = PresetCameraType.PerspectiveHeroicLeftFacing;
// Apply some additional 3D formatting to make the effect visible
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.Material = PresetMaterialType.Plastic;
threeDFormat.Lighting = LightRigType.ThreePoint;
threeDFormat.LightingDirection = LightRigDirectionType.Top;
// Display the new PresetCameraType value
Console.WriteLine("New PresetCameraType: " + threeDFormat.PresetCameraType);
// Save the workbook to show the effect
workbook.Save("ThreeDFormatPresetCameraTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [PresetCameraType](../../presetcameratype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
