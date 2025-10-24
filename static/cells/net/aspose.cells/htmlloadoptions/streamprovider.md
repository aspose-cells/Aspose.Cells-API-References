##HtmlLoadOptions.StreamProvider
HtmlLoadOptions property. Gets or sets the StreamProviderImportHtmlFile for importing objects
## HtmlLoadOptions.StreamProvider property
Gets or sets the StreamProviderImportHtmlFile for importing objects.
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
public class HtmlLoadOptionsPropertyStreamProviderDemo : IStreamProvider
{
public void InitStream(StreamProviderOptions options)
{
// Initialize stream as needed
}
public Stream ProvideStream(StreamProviderOptions options)
{
// Return a stream for reading/writing
return File.Open(options.DefaultPath, FileMode.OpenOrCreate, FileAccess.ReadWrite);
}
public void CloseStream(StreamProviderOptions options)
{
// Close the stream
options.Stream.Close();
}
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
workbook.Worksheets[0].Cells["A1"].PutValue("StreamProvider Demo");
// Save with custom StreamProvider
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
workbook.Save("output.html", saveOptions);
// Load with custom StreamProvider
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
loadOptions.StreamProvider = new HtmlLoadOptionsPropertyStreamProviderDemo();
Workbook loadedWorkbook = new Workbook("output.html", loadOptions);
// Verify loaded data
Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
}
}
}
```
### See Also
* interface [IStreamProvider](../../istreamprovider/)
* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
