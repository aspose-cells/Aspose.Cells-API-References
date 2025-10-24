##ThreeDFormat.Material
ThreeDFormat property. Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape
## ThreeDFormat.Material property
Represents the preset material which is combined with the lighting properties to give the final look and feel of a shape.
```csharp
public PresetMaterialType Material { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyMaterialDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 10, 10, 200, 100, 0, 0);
shape.Text = "3D Material Demo";
// Access the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Display current material value
Console.WriteLine("Current Material value: " + threeDFormat.Material);
// Set different material types and observe the effects
threeDFormat.Material = PresetMaterialType.Metal;
Console.WriteLine("Material changed to Metal");
threeDFormat.Material = PresetMaterialType.Plastic;
Console.WriteLine("Material changed to Plastic");
threeDFormat.Material = PresetMaterialType.Matte;
Console.WriteLine("Material changed to Matte");
// Configure other 3D properties to better see the material effect
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.PresetCameraType = PresetCameraType.PerspectiveFront;
threeDFormat.RotationX = 20;
threeDFormat.RotationY = 30;
// Save the workbook with the 3D effects
workbook.Save("ThreeDFormatMaterialDemo.xlsx");
}
}
}
```
### See Also
* enum [PresetMaterialType](../../presetmaterialtype/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
