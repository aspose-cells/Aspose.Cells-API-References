##Enum ColorDepth
Aspose.Cells.Rendering.ColorDepth enum. Enumerates Bit Depth Type for tiff image
## ColorDepth enumeration
Enumerates Bit Depth Type for tiff image.
```csharp
public enum ColorDepth
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Default value, not set value. |
| Format1bpp | `1` | 1 bit per pixel |
| Format4bpp | `4` | 4 bits per pixel |
| Format8bpp | `8` | 8 bits per pixel |
| Format24bpp | `24` | 24 bits per pixel |
| Format32bpp | `32` | 32 bits per pixel |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using System;
public class RenderingClassColorDepthDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
worksheet.Cells["B2"].PutValue(12345);
// Configure TIFF image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Tiff;
options.TiffColorDepth = ColorDepth.Format8bpp;
// Render worksheet to TIFF with specified color depth
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "output_8bpp.tiff");
// Demonstrate another color depth variant
options.TiffColorDepth = ColorDepth.Format24bpp;
renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "output_24bpp.tiff");
Console.WriteLine("TIFF files created with different color depths.");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
