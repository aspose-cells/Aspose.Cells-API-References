##RenderingWatermark.Image
RenderingWatermark property. Gets image of the watermark
## RenderingWatermark.Image property
Gets image of the watermark.
```csharp
public byte[] Image { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.IO;
public class RenderingWatermarkPropertyImageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Load image data from file
byte[] originalImage = File.ReadAllBytes("watermark.png");
// Create image-based watermark with initial image
RenderingWatermark watermark = new RenderingWatermark(originalImage);
Console.WriteLine("Initial image size: " + watermark.Image.Length + " bytes");
// Modify watermark properties
watermark.Rotation = 45f;
watermark.Opacity = 0.5f;
watermark.ScaleToPagePercent = 75;
watermark.IsBackground = true;
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;
// Create PDF save options with watermark
PdfSaveOptions pdfOptions = new PdfSaveOptions();
pdfOptions.Watermark = watermark; // Fixed property name
// Save to PDF with watermarked output
workbook.Save("WatermarkedOutput.pdf", pdfOptions);
// Create new watermark with different image
byte[] updatedImage = File.ReadAllBytes("updated_watermark.png");
RenderingWatermark newWatermark = new RenderingWatermark(updatedImage);
Console.WriteLine("Updated image size: " + newWatermark.Image.Length + " bytes");
// Save with new watermark
pdfOptions.Watermark = newWatermark; // Fixed property name
workbook.Save("UpdatedWatermark.pdf", pdfOptions);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
