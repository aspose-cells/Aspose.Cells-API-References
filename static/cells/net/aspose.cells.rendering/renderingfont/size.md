##RenderingFont.Size
RenderingFont property. Gets size of the font in points
## RenderingFont.Size property
Gets size of the font in points.
```csharp
public float Size { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingFontPropertySizeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Create initial font and demonstrate reading Size property
RenderingFont smallFont = new RenderingFont("Arial", 12);
Console.WriteLine("Initial font size: " + smallFont.Size);
// Create watermark with initial font size
PdfSaveOptions optionsSmall = new PdfSaveOptions
{
Watermark = new RenderingWatermark("CONFIDENTIAL", smallFont)
};
workbook.Save("SmallWatermark.pdf", optionsSmall);
// Create new font with larger size
RenderingFont largeFont = new RenderingFont("Arial", 24);
Console.WriteLine("Modified font size: " + largeFont.Size);
// Create watermark with larger font size
PdfSaveOptions optionsLarge = new PdfSaveOptions
{
Watermark = new RenderingWatermark("CONFIDENTIAL", largeFont)
};
workbook.Save("LargeWatermark.pdf", optionsLarge);
}
}
}
```
### See Also
* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
