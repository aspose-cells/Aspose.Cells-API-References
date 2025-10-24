##ImageOrPrintOptions.Transparent
ImageOrPrintOptions property. Indicates if the background of generated image should be transparent
## ImageOrPrintOptions.Transparent property
Indicates if the background of generated image should be transparent.
```csharp
public bool Transparent { get; set; }
```
### Remarks
The default value is false. That means the background of the generated images is white.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyTransparentDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Transparent Image Demo");
// Set HTML save options with transparent PNG image
HtmlSaveOptions options = new HtmlSaveOptions();
options.ImageOptions.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.ImageOptions.Transparent = true;
options.ExportImagesAsBase64 = true;
// Save the workbook with transparent image options
workbook.Save("output.html", options);
Console.WriteLine("HTML with transparent images saved successfully.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
