##ImageOrPrintOptions.EmbededImageNameInSvg
ImageOrPrintOptions property. Indicate the filename of embedded image in svg. This should be full path with directory like cxpsEmbedded
## ImageOrPrintOptions.EmbededImageNameInSvg property
Indicate the filename of embedded image in svg. This should be full path with directory like "c:\\xpsEmbedded"
```csharp
[Obsolete("Images are now always embedded in Svg with base64 format, please remove this property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string EmbededImageNameInSvg { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please remove this property because images are now always embedded in Svg with base64 format. This property will be removed 12 months later since April 2025. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Rendering;
using System;
using System.IO;
public class ImageOrPrintOptionsPropertyEmbededImageNameInSvgDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Generate a simple in-memory image and add to worksheet
byte[] redPngBytes = Convert.FromBase64String("iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVR42mNkYPhfDwAChwGA60e6kgAAAABJRU5ErkJggg==");
worksheet.Pictures.Add(0, 0, new MemoryStream(redPngBytes));
// Create image rendering options with SVG format
ImageOrPrintOptions options = new ImageOrPrintOptions
{
ImageType = ImageType.Svg
};
// Display current embedded image path
Console.WriteLine("Initial EmbededImageNameInSvg: " + options.EmbededImageNameInSvg);
// Configure new embedded image directory
string imageDir = "svg_embedded_images/";
options.EmbededImageNameInSvg = imageDir;
Directory.CreateDirectory(imageDir);
// Render worksheet to SVG with configured options
SheetRender renderer = new SheetRender(worksheet, options);
renderer.ToImage(0, "worksheet_output.svg");
Console.WriteLine("Generated SVG with embedded images in: " + Path.GetFullPath(imageDir));
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
