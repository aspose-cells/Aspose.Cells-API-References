##HtmlSaveOptions.ImageOptions
HtmlSaveOptions property. Get the ImageOrPrintOptions object before exporting
## HtmlSaveOptions.ImageOptions property
Get the ImageOrPrintOptions object before exporting
```csharp
public ImageOrPrintOptions ImageOptions { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyImageOptionsDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Export");
// Set HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportImagesAsBase64 = true;
// Configure image options
ImageOrPrintOptions imageOptions = saveOptions.ImageOptions;
imageOptions.ImageType = ImageType.Svg;
imageOptions.HorizontalResolution = 300;
imageOptions.VerticalResolution = 300;
// Save the workbook with HTML options
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file saved with SVG images.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../../../aspose.cells.rendering/imageorprintoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
