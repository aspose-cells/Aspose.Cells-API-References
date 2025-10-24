##RenderingWatermark.RenderingWatermark
RenderingWatermark constructor. Creates instance of text watermark
## RenderingWatermark(string, RenderingFont) {#constructor_1}
Creates instance of text watermark.
```csharp
public RenderingWatermark(string text, RenderingFont renderingFont)
```
| Parameter | Type | Description |
| --- | --- | --- |
| text | String | watermark text |
| renderingFont | RenderingFont | watermark font |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class RenderingWatermarkMethodCtorWithStringRenderingFontDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create a RenderingFont object
RenderingFont renderingFont = new RenderingFont("Arial", 12)
{
Bold = true,
Color = Color.Blue
};
// Create a RenderingWatermark object using the #ctor(string, RenderingFont)
RenderingWatermark watermark = new RenderingWatermark("DEMO WATERMARK", renderingFont)
{
Rotation = 45,
Opacity = 0.3f
};
// Create PdfSaveOptions and set the watermark
PdfSaveOptions saveOptions = new PdfSaveOptions
{
Watermark = watermark
};
// Save the workbook with watermark
workbook.Save("WatermarkDemo.pdf", saveOptions);
}
}
}
```
### See Also
* class [RenderingFont](../../renderingfont/)
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
## RenderingWatermark(byte[]) {#constructor}
Creates instance of image watermark.
```csharp
public RenderingWatermark(byte[] imageData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| imageData | Byte[] |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class RenderingWatermarkMethodCtorWithByteArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Prepare image data for watermark
string imagePath = "watermark.png";
if (!File.Exists(imagePath))
{
Console.WriteLine($"Image file not found: {imagePath}");
return;
}
try
{
byte[] imageData = File.ReadAllBytes(imagePath);
// Create RenderingWatermark with Byte[] constructor
RenderingWatermark watermark = new RenderingWatermark(imageData);
// Configure watermark properties
watermark.Rotation = 45;
watermark.Opacity = 0.5f;
watermark.ScaleToPagePercent = 50;
watermark.IsBackground = true;
watermark.HAlignment = TextAlignmentType.Center;
watermark.VAlignment = TextAlignmentType.Center;
// Create PDF save options and apply watermark
PdfSaveOptions saveOptions = new PdfSaveOptions();
saveOptions.Watermark = watermark; // Fixed property name
// Save workbook with watermark effect
workbook.Save("WatermarkOutput.pdf", saveOptions);
Console.WriteLine("Watermark applied successfully using Byte[] constructor. Output saved to WatermarkOutput.pdf");
}
catch (FileNotFoundException ex)
{
Console.WriteLine($"Error loading image file: {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RenderingWatermark constructor: {ex.Message}");
}
}
}
}
```
### See Also
* class [RenderingWatermark](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
