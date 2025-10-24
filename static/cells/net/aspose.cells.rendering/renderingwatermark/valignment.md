##RenderingWatermark.VAlignment
RenderingWatermark property. Gets or sets vertical alignment of the watermark to the page
## RenderingWatermark.VAlignment property
Gets or sets vertical alignment of the watermark to the page.
```csharp
public TextAlignmentType VAlignment { get; set; }
```
### Remarks
Only Top, Center, Bottom is valid. Default is Top.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingWatermarkPropertyVAlignmentDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Watermark VAlignment Demo");
// Create PDF save options
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Create and configure watermark with different VAlignment settings
RenderingFont font = new RenderingFont("Arial", 48)
{
Bold = true,
Color = System.Drawing.Color.Red
};
// Create watermark with vertical alignment set to Center
RenderingWatermark watermark = new RenderingWatermark("CENTER ALIGNED", font)
{
VAlignment = TextAlignmentType.Center,
HAlignment = TextAlignmentType.Center,
Opacity = 0.5f
};
pdfSaveOptions.Watermark = watermark;
// Save the workbook with watermark
workbook.Save("WatermarkVAlignmentDemo.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* enum [TextAlignmentType](../../../aspose.cells/textalignmenttype/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
