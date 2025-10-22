##HtmlSaveOptions.StreamProvider
HtmlSaveOptions property. Gets or sets the IStreamProvider for exporting objects
## HtmlSaveOptions.StreamProvider property
Gets or sets the IStreamProvider for exporting objects.
```csharp
public IStreamProvider StreamProvider { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class HtmlSaveOptionsPropertyStreamProviderDemo
{
public static void Run()
{
// Create a temporary directory for output
string outputDir = Path.Combine(Path.GetTempPath(), "AsposeStreamProviderDemo");
Directory.CreateDirectory(outputDir);
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("StreamProvider Demo");
// Configure HTML save options with custom stream provider
HtmlSaveOptions options = new HtmlSaveOptions();
options.StreamProvider = new ExportStreamProvider(outputDir);
// Save the workbook as HTML
string outputPath = Path.Combine(outputDir, "output.html");
workbook.Save(outputPath, options);
Console.WriteLine($"File saved with StreamProvider to: {outputPath}");
}
}
public class ExportStreamProvider : IStreamProvider
{
private readonly string _outputDirectory;
public ExportStreamProvider(string outputDirectory)
{
_outputDirectory = outputDirectory;
}
public void InitStream(StreamProviderOptions options)
{
// Initialization if needed
}
public Stream GetStream(StreamProviderOptions options)
{
string filePath = Path.Combine(_outputDirectory, options.CustomPath);
return new FileStream(filePath, FileMode.Create);
}
public void CloseStream(StreamProviderOptions options)
{
// Implementation as required by interface
}
}
}
```
### See Also
* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
