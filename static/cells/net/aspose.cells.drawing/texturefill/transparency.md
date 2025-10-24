##TextureFill.Transparency
TextureFill property. Returns or sets the degree of transparency of the area as a value from 0.0 opaque through 1.0 clear
## TextureFill.Transparency property
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```csharp
public double Transparency { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TextureFillPropertyTransparencyDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape to the worksheet
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
// Set fill type to texture
shape.Fill.FillType = FillType.Texture;
// Access the texture fill properties
TextureFill textureFill = shape.Fill.TextureFill;
// Set a built-in texture type
textureFill.Type = TextureType.BlueTissuePaper;
// Display initial transparency value
Console.WriteLine("Initial Transparency: " + textureFill.Transparency);
// Change transparency to 70% (0.0 = opaque, 1.0 = fully transparent)
textureFill.Transparency = 0.7;
Console.WriteLine("Updated Transparency: " + textureFill.Transparency);
// Save the workbook with visible transparency effect
workbook.Save("TextureFillTransparencyDemo.xlsx");
}
}
}
```
### See Also
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
