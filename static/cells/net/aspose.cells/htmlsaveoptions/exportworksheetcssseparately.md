##HtmlSaveOptions.ExportWorksheetCSSSeparately
HtmlSaveOptions property. Indicating whether export the worksheet css separately.The default value is false
## HtmlSaveOptions.ExportWorksheetCSSSeparately property
Indicating whether export the worksheet css separately.The default value is false.
```csharp
public bool ExportWorksheetCSSSeparately { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyExportWorksheetCSSSeparatelyDemo
{
public static void Run()
{
// Create a sample workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Data");
// Set HTML save options with ExportWorksheetCSSSeparately
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.ExportWorksheetCSSSeparately = true;
// Save the workbook as HTML
string outputPath = Path.Combine(Environment.GetFolderPath(Environment.SpecialFolder.Desktop), "output.html");
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file with separate CSS saved to: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
