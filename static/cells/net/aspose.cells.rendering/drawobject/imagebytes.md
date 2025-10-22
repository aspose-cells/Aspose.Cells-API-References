##DrawObject.ImageBytes
DrawObject property. Indicates image bytes of rendered Chart Shape when rendering
## DrawObject.ImageBytes property
Indicates image bytes of rendered Chart, Shape when rendering.
```csharp
public byte[] ImageBytes { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class DrawObjectPropertyImageBytesDemo
{
// Custom event handler to capture image bytes
private class ImageBytesHandler : DrawObjectEventHandler
{
public byte[] CapturedImageBytes { get; private set; }
public override void Draw(DrawObject drawObject, float x, float y, float width, float height)
{
if (drawObject.Type == DrawObjectEnum.Image)
{
CapturedImageBytes = drawObject.ImageBytes;
Console.WriteLine($"Captured image size: {CapturedImageBytes?.Length ?? 0} bytes");
}
}
}
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Base64 encoded 1x1 red pixel PNG
byte[] generatedImageBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
// Add generated image to worksheet using a stream
using (MemoryStream imageStream = new MemoryStream(generatedImageBytes))
{
worksheet.Pictures.Add(0, 0, imageStream);
}
// Set up rendering options
ImageOrPrintOptions renderOptions = new ImageOrPrintOptions();
renderOptions.ImageType = ImageType.Png;
// Create handler instance and assign to options
var imageHandler = new ImageBytesHandler();
renderOptions.DrawObjectEventHandler = imageHandler;
SheetRender sheetRenderer = new SheetRender(worksheet, renderOptions);
// Render worksheet to trigger DrawObject event using a dummy stream
using (MemoryStream dummyStream = new MemoryStream())
{
sheetRenderer.ToImage(0, dummyStream);
}
// Add captured image to worksheet if available
byte[] capturedImageBytes = imageHandler.CapturedImageBytes;
if (capturedImageBytes != null)
{
int newRowPosition = worksheet.Cells.MaxDataRow + 2;
using (MemoryStream capturedStream = new MemoryStream(capturedImageBytes))
{
worksheet.Pictures.Add(newRowPosition, 0, capturedStream);
}
}
// Save modified workbook
workbook.Save("ImageBytesDemo.xlsx");
}
}
}
```
### See Also
* class [DrawObject](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
