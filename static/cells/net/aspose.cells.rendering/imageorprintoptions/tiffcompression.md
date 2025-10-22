##ImageOrPrintOptions.TiffCompression
ImageOrPrintOptions property. Gets or sets the type of compression to apply only when saving pages to the Tiff format
## ImageOrPrintOptions.TiffCompression property
Gets or sets the type of compression to apply only when saving pages to the `Tiff` format.
```csharp
public TiffCompression TiffCompression { get; set; }
```
### Remarks
Has effect only when saving to TIFF. The default value is Lzw.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyTiffCompressionDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("TIFF Compression Test");
// Set image options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = ImageType.Tiff;
options.HorizontalResolution = 300;
options.VerticalResolution = 300;
// Test different compression types
string outputPath = "OutputTIFF_";
options.TiffCompression = TiffCompression.CompressionNone;
SaveAsTiff(workbook, options, outputPath + "None.tiff");
options.TiffCompression = TiffCompression.CompressionRle;
SaveAsTiff(workbook, options, outputPath + "Rle.tiff");
options.TiffCompression = TiffCompression.CompressionLZW;
SaveAsTiff(workbook, options, outputPath + "LZW.tiff");
options.TiffCompression = TiffCompression.CompressionCCITT3;
SaveAsTiff(workbook, options, outputPath + "CCITT3.tiff");
options.TiffCompression = TiffCompression.CompressionCCITT4;
SaveAsTiff(workbook, options, outputPath + "CCITT4.tiff");
}
private static void SaveAsTiff(Workbook workbook, ImageOrPrintOptions options, string fileName)
{
WorkbookRender renderer = new WorkbookRender(workbook, options);
renderer.ToImage(fileName);
}
}
}
```
### See Also
* enum [TiffCompression](../../tiffcompression/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
