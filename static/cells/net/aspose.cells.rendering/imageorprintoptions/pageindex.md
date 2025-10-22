##ImageOrPrintOptions.PageIndex
ImageOrPrintOptions property. Gets or sets the 0based index of the first page to save
## ImageOrPrintOptions.PageIndex property
Gets or sets the 0-based index of the first page to save.
```csharp
public int PageIndex { get; set; }
```
### Remarks
Default is 0.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class ImageOrPrintOptionsPropertyPageIndexDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to multiple pages
for (int i = 0; i < 50; i++)
{
worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
}
// Set up image/print options
ImageOrPrintOptions options = new ImageOrPrintOptions();
options.PageIndex = 1; // Start from second page (0-based index would be 1)
options.PageCount = 1; // Only process one page
// Create sheet render for the first worksheet
SheetRender render = new SheetRender(worksheet, options);
// Save to PDF using the correct API method
render.ToImage(0, "output.pdf");
Console.WriteLine("Saved page 2 to PDF successfully.");
}
}
}
```
### See Also
* class [ImageOrPrintOptions](../)
* namespace [Aspose.Cells.Rendering](../../../aspose.cells.rendering/)
* assembly [Aspose.Cells](../../../)
