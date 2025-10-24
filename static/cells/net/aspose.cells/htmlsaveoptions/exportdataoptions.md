##HtmlSaveOptions.ExportDataOptions
HtmlSaveOptions property. Indicating the rule of exporting html file data.The default value is All
## HtmlSaveOptions.ExportDataOptions property
Indicating the rule of exporting html file data.The default value is All.
```csharp
public HtmlExportDataOptions ExportDataOptions { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportDataOptionsDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create HTML save options and set ExportDataOptions
HtmlSaveOptions htmlSaveOptions = new HtmlSaveOptions();
htmlSaveOptions.ExportDataOptions = HtmlExportDataOptions.All;
// Save as HTML with all data export options
workbook.Save("output.html", htmlSaveOptions);
Console.WriteLine("HTML file saved with ExportDataOptions.All");
}
}
}
```
### See Also
* enum [HtmlExportDataOptions](../../htmlexportdataoptions/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
