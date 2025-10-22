##HtmlSaveOptions.IsExpImageToTempDir
HtmlSaveOptions property. Indicates whether exporting image files to temp directory. Only for saving to html stream
## HtmlSaveOptions.IsExpImageToTempDir property
Indicates whether exporting image files to temp directory. Only for saving to html stream.
```csharp
public bool IsExpImageToTempDir { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyIsExpImageToTempDirDemo
{
public static void Run()
{
// Create a sample workbook with an image
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample image to the worksheet
worksheet.Pictures.Add(0, 0, "https://www.aspose.com/templates/aspose/App_Themes/V3/images/cells/header/aspose_cells-for-net.png");
// Set HTML save options with IsExpImageToTempDir enabled
HtmlSaveOptions options = new HtmlSaveOptions();
options.IsExpImageToTempDir = true;
options.ExportImagesAsBase64 = false; // Ensure images are exported as separate files
// Save the workbook as HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML saved with images exported to temp directory.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
