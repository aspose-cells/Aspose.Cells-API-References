##HtmlSaveOptions.WorksheetScalable
HtmlSaveOptions property. Indicates if zooming in or out the html via worksheet zoom level when saving file to html the default value is false
## HtmlSaveOptions.WorksheetScalable property
Indicates if zooming in or out the html via worksheet zoom level when saving file to html, the default value is false.
```csharp
public bool WorksheetScalable { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyWorksheetScalableDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample Data");
// Set HTML save options with WorksheetScalable property
HtmlSaveOptions options = new HtmlSaveOptions();
options.WorksheetScalable = true;
// Save the workbook with HTML options
string outputPath = "output.html";
workbook.Save(outputPath, options);
// Verify the output contains scaling style
string htmlContent = File.ReadAllText(outputPath);
Console.WriteLine("HTML contains scaling: " + htmlContent.Contains("transform: scale"));
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
