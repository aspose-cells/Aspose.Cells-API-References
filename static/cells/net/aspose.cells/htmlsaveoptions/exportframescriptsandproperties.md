##HtmlSaveOptions.ExportFrameScriptsAndProperties
HtmlSaveOptions property. Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel please keep the default value
## HtmlSaveOptions.ExportFrameScriptsAndProperties property
Indicating whether exporting frame scripts and document properties. The default value is true.If you want to import the html or mht file to excel, please keep the default value.
```csharp
public bool ExportFrameScriptsAndProperties { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportFrameScriptsAndPropertiesDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Hello");
worksheet.Cells["B1"].PutValue("World");
// Set HTML save options with ExportFrameScriptsAndProperties
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportFrameScriptsAndProperties = true;
// Save as HTML
workbook.Save("output.html", options);
Console.WriteLine("HTML file saved with ExportFrameScriptsAndProperties enabled.");
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
