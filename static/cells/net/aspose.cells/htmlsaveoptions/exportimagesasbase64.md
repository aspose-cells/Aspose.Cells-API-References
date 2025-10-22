##HtmlSaveOptions.ExportImagesAsBase64
HtmlSaveOptions property. Specifies whether images are saved in Base64 format to HTML MHTML or EPUB
## HtmlSaveOptions.ExportImagesAsBase64 property
Specifies whether images are saved in Base64 format to HTML, MHTML or EPUB.
```csharp
public bool ExportImagesAsBase64 { get; set; }
```
### Remarks
When this property is set to true image data is exported directly on the img elements and separate files are not created.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportImagesAsBase64Demo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an image to the worksheet
worksheet.Pictures.Add(0, 0, "example.jpg");
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set ExportImagesAsBase64 to true to embed images as base64 strings
saveOptions.ExportImagesAsBase64 = true;
// Save the workbook as HTML with embedded images
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML with embedded images saved successfully.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
