##PageSetup.PrintHeadings
PageSetup property. Represents if row and column headings are printed with this page
## PageSetup.PrintHeadings property
Represents if row and column headings are printed with this page.
```csharp
public bool PrintHeadings { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PageSetupPropertyPrintHeadingsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some sample data with headings
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Price");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(2.5);
worksheet.Cells["A3"].PutValue("Orange");
worksheet.Cells["B3"].PutValue(1.8);
// Enable printing of headings
worksheet.PageSetup.PrintHeadings = true;
worksheet.PageSetup.PrintArea = "A1:B3";
// Save as HTML to demonstrate the effect
HtmlSaveOptions saveOptions = new HtmlSaveOptions
{
ExportActiveWorksheetOnly = true,
ExportPrintAreaOnly = true,
ExportGridLines = true,
ExportHeadings = true
};
workbook.Save("PrintHeadingsDemo.html", saveOptions);
Console.WriteLine("Worksheet saved with PrintHeadings enabled.");
}
}
}
```
### See Also
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
