##HtmlSaveOptions.ExportSingleTab
HtmlSaveOptions property. Indicates whether exporting the single tab when the file only has one worksheet. The default value is false
## HtmlSaveOptions.ExportSingleTab property
Indicates whether exporting the single tab when the file only has one worksheet. The default value is false.
```csharp
public bool ExportSingleTab { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportSingleTabDemo
{
public static void Run()
{
// Create a new workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Alice");
worksheet.Cells["B3"].PutValue(25);
// Create HTML save options with ExportSingleTab set to true
HtmlSaveOptions options = new HtmlSaveOptions
{
ExportSingleTab = true,
ExportImagesAsBase64 = true
};
// Save the workbook as HTML
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "SingleTabExport.html");
workbook.Save(outputPath, options);
Console.WriteLine("HTML file with single tab export created successfully: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
