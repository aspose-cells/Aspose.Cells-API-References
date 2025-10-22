##HtmlSaveOptions.AttachedFilesDirectory
HtmlSaveOptions property. The directory that the attached files will be saved to. Only for saving to html stream
## HtmlSaveOptions.AttachedFilesDirectory property
The directory that the attached files will be saved to. Only for saving to html stream.
```csharp
public string AttachedFilesDirectory { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyAttachedFilesDirectoryDemo
{
public static void Run()
{
// Create a temporary directory for demonstration
string tempDir = Path.Combine(Path.GetTempPath(), "AsposeAttachedFilesDemo");
Directory.CreateDirectory(tempDir);
try
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
// Set HTML save options with AttachedFilesDirectory
HtmlSaveOptions options = new HtmlSaveOptions();
options.AttachedFilesDirectory = tempDir;
// Save the workbook as HTML
string outputPath = Path.Combine(tempDir, "output.html");
workbook.Save(outputPath, options);
// Verify the attached files were created
Console.WriteLine("HTML saved with attached files in: " + tempDir);
Console.WriteLine("Attached files exist: " +
File.Exists(Path.Combine(tempDir, "sheet001.htm")));
}
finally
{
// Clean up
Directory.Delete(tempDir, true);
}
}
}
}
```
### See Also
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
