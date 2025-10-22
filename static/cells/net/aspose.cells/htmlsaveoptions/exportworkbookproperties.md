##HtmlSaveOptions.ExportWorkbookProperties
HtmlSaveOptions property. Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
## HtmlSaveOptions.ExportWorkbookProperties property
Indicating whether exporting workbook properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
```csharp
public bool ExportWorkbookProperties { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportWorkbookPropertiesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add some data to the workbook
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World!");
// Set workbook properties
workbook.BuiltInDocumentProperties.Author = "Test Author";
workbook.BuiltInDocumentProperties.Title = "Test Title";
// Create HTML save options
HtmlSaveOptions options = new HtmlSaveOptions();
// Demonstrate ExportWorkbookProperties by setting it to false
options.ExportWorkbookProperties = false;
// Save the workbook as HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with ExportWorkbookProperties set to false");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
