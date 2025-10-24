##RenderingWatermark.IsBackground
RenderingWatermark property. Indicates whether the watermark is placed behind page contents
## RenderingWatermark.IsBackground property
Indicates whether the watermark is placed behind page contents.
```csharp
public bool IsBackground { get; set; }
```
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyIsBackgroundDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["A1"].PutValue("Sample Content");
// Create watermark with IsBackground set to true
RenderingFont font = new RenderingFont("Arial", 36)
{
Color = Color.LightGray
};
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
{
IsBackground = true,
Rotation = 45,
Opacity = 0.2f
};
// Configure save options with watermark
PdfSaveOptions options = new PdfSaveOptions
{
Watermark = watermark
};
// Save with background watermark
workbook.Save("WatermarkIsBackgroundDemo.pdf", options);
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
