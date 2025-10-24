##ImageOrPrintOptions.PrintingPage
ImageOrPrintOptions property. Indicates which pages will not be printed
## ImageOrPrintOptions.PrintingPage property
Indicates which pages will not be printed.
```csharp
public PrintingPageType PrintingPage { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyPrintingPageDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Test Data");
worksheet.Cells["A2"].PutValue("Non-Blank Cell");
worksheet.Cells["A5"].PutValue("Another Non-Blank Cell");
// Create image/print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.PrintingPage = PrintingPageType.IgnoreBlank;
// Render the workbook with the options
WorkbookRender render = new WorkbookRender(workbook, options);
// Output the page count (will ignore blank pages)
Console.WriteLine("Page count with IgnoreBlank: " + render.PageCount);
// Change to default behavior (include all pages)
options.PrintingPage = PrintingPageType.Default;
render = new WorkbookRender(workbook, options);
Console.WriteLine("Page count with Default: " + render.PageCount);
}
}
}
```
### See Also
* enum [PrintingPageType](../../../aspose.cells/printingpagetype/)
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
