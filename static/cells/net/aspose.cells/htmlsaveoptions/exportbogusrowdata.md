##HtmlSaveOptions.ExportBogusRowData
HtmlSaveOptions property. Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel please keep the default value
## HtmlSaveOptions.ExportBogusRowData property
Indicating whether exporting bogus bottom row data. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
```csharp
public bool ExportBogusRowData { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportBogusRowDataDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to cells
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
// Create HTML save options
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
// First export without bogus row data
saveOptions.ExportBogusRowData = false;
workbook.Save("output_without_bogus.html", saveOptions);
// Then export with bogus row data
saveOptions.ExportBogusRowData = true;
workbook.Save("output_with_bogus.html", saveOptions);
// Display the results
Console.WriteLine("HTML files created successfully.");
Console.WriteLine("Check output_without_bogus.html and output_with_bogus.html to see the difference.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
