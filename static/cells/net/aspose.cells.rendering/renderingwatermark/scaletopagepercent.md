##RenderingWatermark.ScaleToPagePercent
RenderingWatermark property. Gets or sets scale relative to target page in percent
## RenderingWatermark.ScaleToPagePercent property
Gets or sets scale relative to target page in percent.
```csharp
public int ScaleToPagePercent { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyScaleToPagePercentDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample worksheet with watermark");
RenderingFont font = new RenderingFont("Arial", 72);
font.Bold = true;
font.Color = Color.LightBlue;
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
watermark.ScaleToPagePercent = 75;
watermark.Opacity = 0.3f;
watermark.IsBackground = true;
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;
workbook.Save("WatermarkDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
