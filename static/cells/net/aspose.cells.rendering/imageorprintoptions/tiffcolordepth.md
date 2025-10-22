##ImageOrPrintOptions.TiffColorDepth
ImageOrPrintOptions property. Gets or sets bit depth to apply only when saving pages to the Tiff format
## ImageOrPrintOptions.TiffColorDepth property
Gets or sets bit depth to apply only when saving pages to the `Tiff` format.
```csharp
public ColorDepth TiffColorDepth { get; set; }
```
### Remarks
Has effect only when saving to TIFF. If TiffCompression is set to CCITT3, CCITT4, this will not take effect, the bit depth of the generated tiff image will be always 1.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
public class ImageOrPrintOptionsPropertyTiffColorDepthDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add formatted content to demonstrate color depth
worksheet.Cells["A1"].PutValue("TIFF Color Depth Demonstration");
Cell cell = worksheet.Cells["B3"];
cell.PutValue("24-bit Color Depth");
Style style = cell.GetStyle();
style.Font.Color = System.Drawing.Color.FromArgb(255, 0, 128, 0);
style.BackgroundColor = System.Drawing.Color.FromArgb(255, 255, 192, 128);
style.Pattern = BackgroundType.Solid;
cell.SetStyle(style);
// Initialize ImageOrPrintOptions for TIFF rendering
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Tiff,
TiffCompression = TiffCompression.CompressionLZW
};
// Display and modify TiffColorDepth
Console.WriteLine($"Initial TiffColorDepth: {options.TiffColorDepth}");
// Render with default depth (1bpp)
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToTiff("DefaultDepthOutput.tiff");
// Change to 24-bit color depth
options.TiffColorDepth = ColorDepth.Format24bpp;
Console.WriteLine($"Modified TiffColorDepth: {options.TiffColorDepth}");
// Render with new depth
renderer.ToTiff("24BitDepthOutput.tiff");
Console.WriteLine("Generated TIFF files with different color depths.");
}
}
}
```
### See Also
* enum [ColorDepth](../../colordepth/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
