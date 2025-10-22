##HtmlSaveOptions.AttachedFilesUrlPrefix
HtmlSaveOptions property. Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream
## HtmlSaveOptions.AttachedFilesUrlPrefix property
Specify the Url prefix of attached files such as image in the html file. Only for saving to html stream.
```csharp
public string AttachedFilesUrlPrefix { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyAttachedFilesUrlPrefixDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test HTML Export");
// Set HTML save options with AttachedFilesUrlPrefix
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html);
saveOptions.AttachedFilesUrlPrefix = "www.aspose.com";
// Save the workbook with HTML options
string outputPath = "output.html";
workbook.Save(outputPath, saveOptions);
Console.WriteLine("HTML file saved with AttachedFilesUrlPrefix: " + saveOptions.AttachedFilesUrlPrefix);
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
