##RenderingWatermark.HAlignment
RenderingWatermark property. Gets or sets horizontal alignment of the watermark to the page
## RenderingWatermark.HAlignment property
Gets or sets horizontal alignment of the watermark to the page.
```csharp
public TextAlignmentType HAlignment { get; set; }
```
### Remarks
Only Left, Center, Right is valid. Default is Left.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyHAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Watermark HAlignment Demo");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Create and configure watermark with different HAlignment settings
RenderingFont font = new RenderingFont("Arial", 48)
{
Bold = true,
Color = System.Drawing.Color.Blue
};
// Create watermark with Center alignment
RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
{
HAlignment = TextAlignmentType.Center,
VAlignment = TextAlignmentType.Center,
Opacity = 0.5f
};
pdfSaveOptions.Watermark = watermark;
// Save with center-aligned watermark
workbook.Save("WatermarkCenterAlignment.pdf", pdfSaveOptions);
// Change to Left alignment
watermark.HAlignment = TextAlignmentType.Left;
workbook.Save("WatermarkLeftAlignment.pdf", pdfSaveOptions);
// Change to Right alignment
watermark.HAlignment = TextAlignmentType.Right;
workbook.Save("WatermarkRightAlignment.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
