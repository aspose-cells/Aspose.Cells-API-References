##Enum TiffCompression
Aspose.Cells.Rendering.TiffCompression enum. Specifies what type of compression to apply when saving images into TIFF format file
## TiffCompression enumeration
Specifies what type of compression to apply when saving images into TIFF format file.
```csharp
public enum TiffCompression
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| CompressionNone | `0` | Specifies no compression. |
| CompressionRle | `1` | Specifies the RLE compression scheme. |
| CompressionLZW | `2` | Specifies the LZW compression scheme. |
| CompressionCCITT3 | `3` | Specifies the CCITT3 compression scheme. |
| CompressionCCITT4 | `4` | Specifies the CCITT4 compression scheme. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class RenderingClassTiffCompressionDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
ws.Cells["A1"].PutValue("TIFF Compression Test");
ws.Cells["A2"].PutValue(DateTime.Now.ToString());
// Set image options
ImageOrPrintOptions imgOpt = new ImageOrPrintOptions();
imgOpt.HorizontalResolution = 300;
imgOpt.VerticalResolution = 300;
imgOpt.ImageType = ImageType.Tiff;
// Test different compression types
string outputPath = "output_compression_";
// LZW Compression
imgOpt.TiffCompression = TiffCompression.CompressionLZW;
new WorkbookRender(wb, imgOpt).ToImage(outputPath + "LZW.tiff");
// CCITT3 Compression
imgOpt.TiffCompression = TiffCompression.CompressionCCITT3;
new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT3.tiff");
// CCITT4 Compression
imgOpt.TiffCompression = TiffCompression.CompressionCCITT4;
new WorkbookRender(wb, imgOpt).ToImage(outputPath + "CCITT4.tiff");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Rendering](../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../)
