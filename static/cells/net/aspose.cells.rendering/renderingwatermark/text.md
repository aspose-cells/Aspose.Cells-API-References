##RenderingWatermark.Text
RenderingWatermark property. Gets text of the watermark
## RenderingWatermark.Text property
Gets text of the watermark.
```csharp
public string Text { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingWatermarkPropertyTextDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create rendering font for watermark text
RenderingFont font = new RenderingFont("Arial", 36);
// Initialize text watermark with font configuration
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
// Display current watermark text
Console.WriteLine("Watermark Text: " + watermark.Text);
// Configure watermark appearance
watermark.Rotation = 45f;
watermark.Opacity = 0.3f;
watermark.IsBackground = true;
watermark.ScaleToPagePercent = 150;
// Apply watermark to PDF save options
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark; // Fixed property name
// Save to PDF to visualize watermark effects
workbook.Save("WatermarkDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
