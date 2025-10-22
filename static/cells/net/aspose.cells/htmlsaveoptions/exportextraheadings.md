##HtmlSaveOptions.ExportExtraHeadings
HtmlSaveOptions property. Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel please keep the default value
## HtmlSaveOptions.ExportExtraHeadings property
Indicates whether exporting extra headings when the length of text is longer than max display column. The default value is false. If you want to import the html file to excel, please keep the default value.
```csharp
public bool ExportExtraHeadings { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportExtraHeadingsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data and extra headings
worksheet.Cells["A1"].PutValue("Main Heading");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
worksheet.Cells["A3"].PutValue("Data3");
worksheet.Cells["B3"].PutValue("Data4");
// Set extra headings (rows and columns)
worksheet.Cells["Z1"].PutValue("Extra Column Heading");
worksheet.Cells["A100"].PutValue("Extra Row Heading");
// Configure HTML save options with ExportExtraHeadings
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportHeadings = true;
saveOptions.ExportExtraHeadings = true;
// Save to HTML
workbook.Save("output.html", saveOptions);
Console.WriteLine("HTML exported with extra headings.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
