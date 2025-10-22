##ThreeDFormat.ExtrusionColor
ThreeDFormat property. Gets the extrusion color on a shape
## ThreeDFormat.ExtrusionColor property
Gets the extrusion color on a shape.
```csharp
public CellsColor ExtrusionColor { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class ThreeDFormatPropertyExtrusionColorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape to demonstrate 3D formatting
Shape shape = worksheet.Shapes.AddShape(MsoDrawingType.TextBox, 1, 1, 0, 0, 200, 100);
shape.Text = "3D ExtrusionColor Demo";
// Get the ThreeDFormat of the shape
ThreeDFormat threeDFormat = shape.ThreeDFormat;
// Configure basic 3D properties to make extrusion visible
threeDFormat.ExtrusionHeight = 20;
threeDFormat.ContourWidth = 2;
threeDFormat.Material = PresetMaterialType.Plastic;
try
{
// Get and display the ExtrusionColor value
CellsColor extrusionColor = threeDFormat.ExtrusionColor;
Console.WriteLine("ExtrusionColor properties:");
Console.WriteLine($"Type: {extrusionColor.Type}");
Console.WriteLine($"Color (RGB): {extrusionColor.Color}");
Console.WriteLine($"Transparency: {extrusionColor.Transparency}");
// Save the workbook to see the 3D effects
workbook.Save("ThreeDFormatExtrusionColorDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [ThreeDFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
