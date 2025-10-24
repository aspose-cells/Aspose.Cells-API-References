##HtmlSaveOptions.ExportRowColumnHeadings
HtmlSaveOptions property. Indicates whether exports sheets row and column headings when saving to HTML files
## HtmlSaveOptions.ExportRowColumnHeadings property
Indicates whether exports sheet's row and column headings when saving to HTML files.
```csharp
public bool ExportRowColumnHeadings { get; set; }
```
### Remarks
The default value is false.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportRowColumnHeadingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to cells
worksheet.Cells["A1"].PutValue("Item");
worksheet.Cells["B1"].PutValue("Quantity");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(15);
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
// Set ExportRowColumnHeadings to false (default is true)
saveOptions.ExportRowColumnHeadings = false;
// Save the workbook with headings disabled
workbook.Save("output_without_headings.html", saveOptions);
// Now enable headings and save again
saveOptions.ExportRowColumnHeadings = true;
workbook.Save("output_with_headings.html", saveOptions);
Console.WriteLine("HTML files saved with different heading visibility settings.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
