##HtmlSaveOptions.ImageScalable
HtmlSaveOptions property. Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true
## HtmlSaveOptions.ImageScalable property
Indicates whether using scalable unit to describe the image width when using scalable unit to describe the column width. The default value is true.
```csharp
public bool ImageScalable { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyImageScalableDemo
{
public static void Run()
{
// Create a sample workbook with an image
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample image to the worksheet
int imgIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Aspose.Cells.Drawing.Picture picture = worksheet.Pictures[imgIndex];
// Set HTML save options with ImageScalable property
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ImageScalable = false; // Images won't scale with the HTML content
// Save the workbook as HTML
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML file saved with ImageScalable set to false.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
