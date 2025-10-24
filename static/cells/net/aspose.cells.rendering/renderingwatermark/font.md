##RenderingWatermark.Font
RenderingWatermark property. Gets font of the watermark
## RenderingWatermark.Font property
Gets font of the watermark.
```csharp
public RenderingFont Font { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingWatermarkPropertyFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create a rendering font and set initial properties
RenderingFont font = new RenderingFont("Arial", 24);
// Create a text watermark with the rendering font
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
// Display initial font properties
Console.WriteLine("Initial Font Name: " + watermark.Font.Name);
Console.WriteLine("Initial Font Size: " + watermark.Font.Size);
Console.WriteLine("Initial Bold Status: " + watermark.Font.Bold);
// Modify font properties through the RenderingFont reference
font.Bold = true;
// Display updated font properties from watermark
Console.WriteLine("\nUpdated Font Name: " + watermark.Font.Name);
Console.WriteLine("Updated Font Size: " + watermark.Font.Size);
Console.WriteLine("Updated Bold Status: " + watermark.Font.Bold);
// Configure watermark display properties
watermark.Opacity = 0.5f;
watermark.Rotation = 45;
watermark.IsBackground = true;
// Create PDF save options and assign watermark
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
pdfSaveOptions.Watermark = watermark;
// Save workbook with watermarked PDF to show font changes
workbook.Save("RenderingWatermarkFontDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
