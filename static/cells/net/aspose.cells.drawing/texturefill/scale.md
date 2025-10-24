##TextureFill.Scale
TextureFill property. Gets and sets the picture format scale
## TextureFill.Scale property
Gets and sets the picture format scale.
```csharp
public double Scale { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class TextureFillPropertyScaleDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a shape and get its fill format
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 10, 10, 500, 300);
FillFormat fillFormat = shape.Fill;
// Configure texture fill
fillFormat.FillType = FillType.Texture;
TextureFill textureFill = fillFormat.TextureFill;
// Load texture image and configure properties
textureFill.ImageData = File.ReadAllBytes("texture.jpg");
textureFill.Type = TextureType.Unknown; // Changed from UserDefined to Unknown
textureFill.IsTiling = true;
// Display and modify scale
Console.WriteLine("Initial Scale: " + textureFill.Scale);
textureFill.Scale = 0.5;
Console.WriteLine("Modified Scale: " + textureFill.Scale);
// Save result
workbook.Save("TextureFillScaleDemo.xlsx");
}
}
}
```
### See Also
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
