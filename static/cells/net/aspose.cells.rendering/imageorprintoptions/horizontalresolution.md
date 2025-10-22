##ImageOrPrintOptions.HorizontalResolution
ImageOrPrintOptions property. Gets or sets the horizontal resolution for generated images in dots per inch
## ImageOrPrintOptions.HorizontalResolution property
Gets or sets the horizontal resolution for generated images, in dots per inch.
```csharp
public int HorizontalResolution { get; set; }
```
### Remarks
The default value is 96.
Setting `HorizontalResolution` and [`VerticalResolution`](../verticalresolution/) effects the width and height of the output image in pixels.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyHorizontalResolutionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Text for Image Rendering");
// Initialize ImageOrPrintOptions
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Png;
// Set horizontal and vertical resolution
options.HorizontalResolution = 192;
options.VerticalResolution = 192;
// Render the worksheet to image with specified resolution
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "WorksheetImage_192dpi.png");
// Demonstrate different resolution
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "WorksheetImage_300dpi.png");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
