##RenderingFont.Name
RenderingFont property. Gets name of the font
## RenderingFont.Name property
Gets name of the font.
```csharp
public string Name { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
public class RenderingFontPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create PDF save options
PdfSaveOptions options = new PdfSaveOptions();
// Create initial rendering font with "Arial"
RenderingFont fontArial = new RenderingFont("Arial", 16);
Console.WriteLine("Initial font name: " + fontArial.Name);
// Create watermark with initial font
RenderingWatermark watermark = new RenderingWatermark("Confidential", fontArial);
watermark.Opacity = 0.5f;
watermark.Rotation = 45;
options.Watermark = watermark;
// Save with initial font watermark
workbook.Save("WatermarkInitial.pdf", options);
// Create new rendering font with "Times New Roman"
RenderingFont fontTimesNewRoman = new RenderingFont("Times New Roman", 16);
Console.WriteLine("\nModified font name: " + fontTimesNewRoman.Name);
// Update watermark with new font
RenderingWatermark updatedWatermark = new RenderingWatermark("Confidential", fontTimesNewRoman);
updatedWatermark.Opacity = 0.5f;
updatedWatermark.Rotation = 45;
options.Watermark = updatedWatermark;
// Save with modified font watermark
workbook.Save("WatermarkModified.pdf", options);
}
}
}
```
### See Also
* class [RenderingFont](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
