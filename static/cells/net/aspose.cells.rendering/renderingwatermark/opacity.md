##RenderingWatermark.Opacity
RenderingWatermark property. Gets or sets opacity of the watermark in range 0 1
## RenderingWatermark.Opacity property
Gets or sets opacity of the watermark in range [0, 1].
```csharp
public float Opacity { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyOpacityDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample content");
RenderingFont font = new RenderingFont("Arial", 72);
font.Bold = true;
font.Color = Color.Blue;
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font);
watermark.Opacity = 0.4f;
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;
watermark.IsBackground = true;
PdfSaveOptions options = new PdfSaveOptions();
options.Watermark = watermark;
workbook.Save("WatermarkOpacityDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
