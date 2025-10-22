##HtmlSaveOptions.PageTitle
HtmlSaveOptions property. The title of the html page. Only for saving to html stream
## HtmlSaveOptions.PageTitle property
The title of the html page. Only for saving to html stream.
```csharp
public string PageTitle { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyPageTitleDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample HTML Export");
// Set HTML save options with PageTitle
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.PageTitle = "My Custom Page Title";
// Save to HTML with the specified title
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file saved with custom page title: " + outputPath);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
