##FillFormat.TextureFill
FillFormat property. Gets TextureFill object
## FillFormat.TextureFill property
Gets `TextureFill` object.
```csharp
public TextureFill TextureFill { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class FillFormatPropertyTextureFillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture shape
string imagePath = Path.Combine("your_image_directory", "texture.png");
int pictureIndex = worksheet.Pictures.Add(0, 0, imagePath);
Shape picture = worksheet.Shapes[pictureIndex];
// Set texture fill properties
picture.Fill.TextureFill.ImageData = File.ReadAllBytes(imagePath);
picture.Fill.TextureFill.IsTiling = true;
picture.Fill.TextureFill.Scale = 0.5;
// Save the workbook
workbook.Save("TextureFillDemo.xlsx");
}
}
}
```
### See Also
* class [TextureFill](../../texturefill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
