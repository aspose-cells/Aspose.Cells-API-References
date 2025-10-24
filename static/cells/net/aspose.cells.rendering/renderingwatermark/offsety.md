##RenderingWatermark.OffsetY
RenderingWatermark property. Gets or sets offset value to VAlignment
## RenderingWatermark.OffsetY property
Gets or sets offset value to [`VAlignment`](../valignment/)
```csharp
public float OffsetY { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyOffsetYDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("OffsetY Demo");
// Create watermark font
RenderingFont font = new RenderingFont("Arial", 24)
{
Color = Color.Red,
Bold = true
};
// Create watermark with different OffsetY values
RenderingWatermark watermark = new RenderingWatermark("VERTICAL OFFSET", font)
{
Rotation = 0,
Opacity = 0.3f,
IsBackground = true,
HAlignment = TextAlignmentType.Center,
VAlignment = TextAlignmentType.Center,
OffsetX = 0,
OffsetY = 100 // Demonstrating OffsetY property
};
// Set save options with watermark
PdfSaveOptions options = new PdfSaveOptions
{
Watermark = watermark
};
// Save with watermark offset
workbook.Save("WatermarkOffsetYDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
