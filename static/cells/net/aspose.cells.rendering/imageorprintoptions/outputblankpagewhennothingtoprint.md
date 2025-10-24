##ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint
ImageOrPrintOptions property. Indicates whether to output a blank page when there is nothing to print
## ImageOrPrintOptions.OutputBlankPageWhenNothingToPrint property
Indicates whether to output a blank page when there is nothing to print.
```csharp
public bool OutputBlankPageWhenNothingToPrint { get; set; }
```
### Remarks
Default is false.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyOutputBlankPageWhenNothingToPrintDemo
{
public static void Run()
{
// Create a new empty workbook
Workbook workbook = new Workbook();
// Access the first worksheet which is empty
Worksheet worksheet = workbook.Worksheets[0];
// Set image or print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.ImageType = Aspose.Cells.Drawing.ImageType.Png;
options.OnePagePerSheet = true;
// Demonstrate OutputBlankPageWhenNothingToPrint property
options.OutputBlankPageWhenNothingToPrint = true;
// Render the sheet
SheetRender renderer = new SheetRender(worksheet, options);
// Output will still produce one blank page due to the property setting
Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=true: " + renderer.PageCount);
// Save the first page to memory stream
MemoryStream stream = new MemoryStream();
renderer.ToImage(0, stream);
Console.WriteLine("Image data length: " + stream.ToArray().Length);
// Now set the property to false
options.OutputBlankPageWhenNothingToPrint = false;
SheetRender renderer2 = new SheetRender(worksheet, options);
// Output will have zero pages now
Console.WriteLine("Page count with OutputBlankPageWhenNothingToPrint=false: " + renderer2.PageCount);
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
