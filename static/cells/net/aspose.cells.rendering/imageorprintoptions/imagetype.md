##ImageOrPrintOptions.ImageType
ImageOrPrintOptions property. Gets or sets the format of the generated images. default value PNG
## ImageOrPrintOptions.ImageType property
Gets or sets the format of the generated images. default value: PNG.
```csharp
public virtual ImageType ImageType { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyImageTypeDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test SVG Image");
// Set HTML save options with SVG image type
HtmlSaveOptions options = new HtmlSaveOptions();
options.ImageOptions.ImageType = ImageType.Svg;
options.ExportActiveWorksheetOnly = true;
// Save the workbook as HTML
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
workbook.Save(outputPath, options);
Console.WriteLine("File saved with SVG images: " + outputPath);
}
}
}
```
### See Also
* enum [ImageType](../../../aspose.cells.drawing/imagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
