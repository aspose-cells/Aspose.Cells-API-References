##RenderingFont.Bold
RenderingFont property. Gets or sets bold for the font
## RenderingFont.Bold property
Gets or sets bold for the font.
```csharp
public bool Bold { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System.Drawing;
namespace AsposeCellsExamples
{
public class RenderingFontPropertyBoldDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Bold Font Example");
// Create a style for the cell
Style style = workbook.CreateStyle();
style.Font.IsBold = true;
worksheet.Cells["A1"].SetStyle(style);
// Create PDF save options with watermark demonstrating bold font
PdfSaveOptions pdfSaveOptions = new PdfSaveOptions();
// Create rendering font with bold property
RenderingFont font = new RenderingFont("Arial", 36)
{
Bold = true,
Color = System.Drawing.Color.Red
};
// Create watermark with bold font
RenderingWatermark watermark = new RenderingWatermark("CONFIDENTIAL", font)
{
HAlignment = TextAlignmentType.Center,
VAlignment = TextAlignmentType.Center,
Opacity = 0.3f
};
pdfSaveOptions.Watermark = watermark;
// Save the workbook
workbook.Save("BoldFontExample.pdf", pdfSaveOptions);
}
}
}
```
### See Also
* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
