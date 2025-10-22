##RenderingWatermark.Rotation
RenderingWatermark property. Gets or sets roation of the watermark in degrees
## RenderingWatermark.Rotation property
Gets or sets roation of the watermark in degrees.
```csharp
public float Rotation { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyRotationDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample data for watermark demo");
// Create font for watermark
RenderingFont font = new RenderingFont("Arial", 72);
font.Color = Color.FromArgb(128, 0, 0, 255);
font.Bold = true;
// Create watermark with rotation
RenderingWatermark watermark = new RenderingWatermark("ROTATED WATERMARK", font);
watermark.Rotation = 45; // 45 degree rotation
watermark.Opacity = 0.5f;
watermark.IsBackground = true;
// Set PDF save options with watermark
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;
// Save with watermark
workbook.Save("WatermarkRotationDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
