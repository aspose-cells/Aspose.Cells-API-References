##TextureFill.PictureFormatType
TextureFill property. Gets and sets the picture format type
## TextureFill.PictureFormatType property
Gets and sets the picture format type.
```csharp
public FillPictureType PictureFormatType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TextureFillPropertyPictureFormatTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape with all required parameters
Shape shape = worksheet.Shapes.AddRectangle(0, 0, 0, 0, 100, 200);
// Set fill type to texture
shape.Fill.FillType = FillType.Texture;
TextureFill textureFill = shape.Fill.TextureFill;
// Load minimal 1x1 pixel PNG image (white)
string base64Image = "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNkYAAAAAYAAjCB0C8AAAAASUVORK5CYII=";
textureFill.ImageData = Convert.FromBase64String(base64Image);
// Display current PictureFormatType
Console.WriteLine("Initial PictureFormatType: " + textureFill.PictureFormatType);
// Change to stacked format and enable tiling
textureFill.PictureFormatType = FillPictureType.Stack;
textureFill.IsTiling = true;
// Add another shape to compare original stretched format
Shape shape2 = worksheet.Shapes.AddRectangle(0, 0, 210, 0, 100, 200);
shape2.Fill.FillType = FillType.Texture;
TextureFill textureFill2 = shape2.Fill.TextureFill;
textureFill2.ImageData = Convert.FromBase64String(base64Image);
// Save the workbook with both texture fill examples
workbook.Save("TextureFillPictureFormatTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FillPictureType](../../fillpicturetype/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
