##ImageOrPrintOptions.TiffBinarizationMethod
ImageOrPrintOptions property. Gets or sets method used while converting images to 1 bpp format when ImageType is Tiff and TiffCompression is equal to Ccitt3 or Ccitt4
## ImageOrPrintOptions.TiffBinarizationMethod property
Gets or sets method used while converting images to 1 bpp format when [`ImageType`](../imagetype/) is Tiff and [`TiffCompression`](../tiffcompression/) is equal to Ccitt3 or Ccitt4.
```csharp
public ImageBinarizationMethod TiffBinarizationMethod { get; set; }
```
### Remarks
The default value is FloydSteinbergDithering.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
using System;
using System.Drawing;
public class ImageOrPrintOptionsPropertyTiffBinarizationMethodDemo
{
public static void Run()
{
// Create workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add gradient data for visual demonstration
for (int i = 0; i < 15; i++)
{
Cell cell = worksheet.Cells[i, 0];
cell.PutValue(i * 7);
Style style = cell.GetStyle();
style.BackgroundColor = Color.FromArgb(i * 18, i * 18, i * 18);
cell.SetStyle(style);
}
// Configure TIFF rendering options
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Tiff,
TiffCompression = TiffCompression.CompressionCCITT3,
TiffColorDepth = ColorDepth.Format1bpp
};
// Display current binarization method
Console.WriteLine("Initial TiffBinarizationMethod: " + options.TiffBinarizationMethod);
// Render with default threshold method
new SheetRender(worksheet, options).ToImage(0, "ThresholdBinarization.tiff");
// Change to Floyd-Steinberg dithering
options.TiffBinarizationMethod = ImageBinarizationMethod.FloydSteinbergDithering;
Console.WriteLine("\nModified TiffBinarizationMethod: " + options.TiffBinarizationMethod);
// Render with new method
new SheetRender(worksheet, options).ToImage(0, "DitheringBinarization.tiff");
Console.WriteLine("\nGenerated TIFF files demonstrate different 1bpp conversion methods.");
}
}
}
```
### See Also
* enum [ImageBinarizationMethod](../../imagebinarizationmethod/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
