##TextureFill.PicFormatOption
TextureFill property. Gets or sets picture format option
## TextureFill.PicFormatOption property
Gets or sets picture format option.
```csharp
public PicFormatOption PicFormatOption { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
public class TextureFillPropertyPicFormatOptionDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a rectangle shape
var shape = worksheet.Shapes.AddRectangle(0, 0, 100, 300, 200, 400);
// Configure texture fill
shape.Fill.FillType = FillType.Texture;
TextureFill textureFill = shape.Fill.TextureFill;
// Set user-defined texture with minimal 1x1 pixel image
// TextureType.UserDefined is not available, removed the invalid assignment
textureFill.ImageData = new byte[] {
0x89, 0x50, 0x4E, 0x47, 0x0D, 0x0A, 0x1A, 0x0A, 0x00, 0x00, 0x00, 0x0D, 0x49, 0x48, 0x44, 0x52,
0x00, 0x00, 0x00, 0x01, 0x00, 0x00, 0x00, 0x01, 0x08, 0x02, 0x00, 0x00, 0x00, 0x90, 0x77, 0x53,
0xDE, 0x00, 0x00, 0x00, 0x01, 0x73, 0x52, 0x47, 0x42, 0x00, 0xAE, 0xCE, 0x1C, 0xE9, 0x00, 0x00,
0x00, 0x04, 0x67, 0x41, 0x4D, 0x41, 0x00, 0x00, 0xB1, 0x8F, 0x0B, 0xFC, 0x61, 0x05, 0x00, 0x00,
0x00, 0x09, 0x70, 0x48, 0x59, 0x73, 0x00, 0x00, 0x0E, 0xC3, 0x00, 0x00, 0x0E, 0xC3, 0x01, 0xC7,
0x6F, 0xA8, 0x64, 0x00, 0x00, 0x00, 0x18, 0x49, 0x44, 0x41, 0x54, 0x18, 0x57, 0x63, 0x60, 0x18,
0x05, 0xA3, 0x60, 0x14, 0x8C, 0x82, 0x51, 0x30, 0x0A, 0x46, 0xC1, 0x28, 0x00, 0x00, 0x01, 0xAD,
0x00, 0x01, 0x8C, 0xF8, 0x2B, 0xD4, 0x00, 0x00, 0x00, 0x00, 0x49, 0x45, 0x4E, 0x44, 0xAE, 0x42,
0x60, 0x82
};
// Enable tiling and show format options
textureFill.IsTiling = true;
// Display initial PicFormatOption state
Console.WriteLine("Initial PicFormatOption: " + (textureFill.PicFormatOption != null ? "Configured" : "Null"));
// Create and apply new format options
textureFill.PicFormatOption = new PicFormatOption
{
Type = FillPictureType.Stretch,
Scale = 0.25,
Left = 15,    // Corrected from LeftOffset
Top = 15,     // Corrected from TopOffset
// ScaleX and ScaleY properties don't exist - removed
};
// Verify property update
Console.WriteLine("Updated PicFormatOption Type: " + textureFill.PicFormatOption.Type);
// Save with modified tiling pattern
workbook.Save("TextureFillPicFormatOptionDemo.xlsx");
}
}
}
```
### See Also
* class [PicFormatOption](../../picformatoption/)
* class [TextureFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
