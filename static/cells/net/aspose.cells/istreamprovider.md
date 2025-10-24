##Interface IStreamProvider
Aspose.Cells.IStreamProvider interface. Represents the exported stream provider
## IStreamProvider interface
Represents the exported stream provider.
```csharp
public interface IStreamProvider
```
## Methods
| Name | Description |
| --- | --- |
| [CloseStream](../../aspose.cells/istreamprovider/closestream/)(StreamProviderOptions) | Closes the stream. |
| [InitStream](../../aspose.cells/istreamprovider/initstream/)(StreamProviderOptions) | Gets the stream. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class IStreamProviderDemo : IStreamProvider
{
// Implementing the InitStream method
public void InitStream(StreamProviderOptions options)
{
string outputDir = "/test/";
string path = outputDir + Path.GetFileName(options.DefaultPath);
options.CustomPath = path;
Directory.CreateDirectory(Path.GetDirectoryName(path));
options.Stream = File.Create(path);
}
// Implementing the CloseStream method
public void CloseStream(StreamProviderOptions options)
{
// Close the stream if it is not null
if (options.Stream != null)
{
options.Stream.Close();
}
}
public static void IStreamProviderExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some data in the worksheet
worksheet.Cells["A1"].PutValue("Hello World");
// Create HtmlSaveOptions and set the StreamProvider
HtmlSaveOptions saveOptions = new HtmlSaveOptions();
saveOptions.StreamProvider = new IStreamProviderDemo();
// Save the workbook to HTML format
workbook.Save("IStreamProviderExample.html", saveOptions);
// Load the workbook from HTML format
HtmlLoadOptions loadOptions = new HtmlLoadOptions();
loadOptions.StreamProvider = new IStreamProviderDemo();
Workbook loadedWorkbook = new Workbook("IStreamProviderExample.html", loadOptions);
// Display the loaded data
Console.WriteLine(loadedWorkbook.Worksheets[0].Cells["A1"].StringValue);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
