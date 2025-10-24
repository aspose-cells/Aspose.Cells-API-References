##HtmlSaveOptions.ExportDocumentProperties
HtmlSaveOptions property. Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel please keep the default value
## HtmlSaveOptions.ExportDocumentProperties property
Indicating whether exporting document properties.The default value is true.If you want to import the html or mht file to excel, please keep the default value.
```csharp
public bool ExportDocumentProperties { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportDocumentPropertiesDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some document properties
workbook.BuiltInDocumentProperties.Author = "Test Author";
workbook.BuiltInDocumentProperties.Title = "Test Document";
// Add sample cell data
worksheet.Cells["A1"].PutValue("Sample HTML Export");
// Create HTML save options and set ExportDocumentProperties to false
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportDocumentProperties = false;
// Save the workbook as HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with document properties export disabled.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
