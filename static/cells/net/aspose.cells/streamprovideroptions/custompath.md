##StreamProviderOptions.CustomPath
StreamProviderOptions property. The user custom pathURL saved in generated html file for the referred source. If not defined by user DefaultPath will be used. For example the sheet data will be saved by user to d/sheet001.htm the url used in the main html file should be d/sheet001.htm or other valid relative path that can be accessed by the main html file
## StreamProviderOptions.CustomPath property
The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.
```csharp
public string CustomPath { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StreamProviderOptionsPropertyCustomPathDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test Data");
// Set up HTML save options with custom stream provider
string outputDir = "output";
Directory.CreateDirectory(outputDir);
HtmlSaveOptions options = new HtmlSaveOptions();
options.ExportActiveWorksheetOnly = true;
// Create custom stream provider with CustomPath
HtmlWithExternalResourcesProvider streamProvider = new HtmlWithExternalResourcesProvider(outputDir);
streamProvider.streamProviderOptions.CustomPath = "resources";
options.StreamProvider = streamProvider;
// Save the workbook
string outputFile = Path.Combine(outputDir, "output.html");
workbook.Save(outputFile, options);
// Verify the custom path was used
string resourcePath = Path.Combine(outputDir, streamProvider.streamProviderOptions.CustomPath);
Console.WriteLine($"Resources should be saved to: {resourcePath}");
}
}
// Simplified custom stream provider implementation
public class HtmlWithExternalResourcesProvider : IStreamProvider
{
public StreamProviderOptions streamProviderOptions = new StreamProviderOptions();
public string _outputDirectory;
public HtmlWithExternalResourcesProvider(string outputDirectory)
{
_outputDirectory = outputDirectory;
}
public void InitStream(StreamProviderOptions options)
{
// Implementation would go here
}
public void CloseStream(StreamProviderOptions options)
{
// Implementation would go here
}
}
}
```
### See Also
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
