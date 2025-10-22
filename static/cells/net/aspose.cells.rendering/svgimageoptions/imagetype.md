##SvgImageOptions.ImageType
SvgImageOptions property. Gets or sets the format of the generated images. default value PNG
## SvgImageOptions.ImageType property
Gets or sets the format of the generated images. default value: PNG.
```csharp
public override ImageType ImageType { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class SvgImageOptionsPropertyImageTypeDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and an image
worksheet.Cells["A1"].PutValue("Embedded Image Type Demonstration");
int pictureIndex = worksheet.Pictures.Add(0, 1, "inputImage.png");
Picture picture = worksheet.Pictures[pictureIndex];
// Create SVG rendering options
SvgImageOptions svgOptions = new SvgImageOptions();
// Display current ImageType (default: PNG)
Console.WriteLine("Current ImageType: " + svgOptions.ImageType);
// Change image format for embedded raster images
svgOptions.ImageType = ImageType.Jpeg;
// Save worksheet content as SVG with different image formats
using (MemoryStream stream = new MemoryStream())
{
picture.ToImage(stream, svgOptions);
File.WriteAllBytes("output_with_jpeg.svg", stream.ToArray());
}
// Reset to PNG format
svgOptions.ImageType = ImageType.Png;
using (MemoryStream stream = new MemoryStream())
{
picture.ToImage(stream, svgOptions);
File.WriteAllBytes("output_with_png.svg", stream.ToArray());
}
Console.WriteLine("SVG files created with different embedded image formats.");
}
}
}
```
### See Also
* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [SvgImageOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
