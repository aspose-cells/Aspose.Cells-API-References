##StreamProviderOptions.DefaultPath
StreamProviderOptions property. The default pathURL saved in generated html file for the referred source. For example the sheet data saved in xxx_files/sheet001.htm the url used in the main html file should be like srcxxx_files/sheet001.htm
## StreamProviderOptions.DefaultPath property
The default path(URL) saved in generated html file for the referred source. For example, the sheet data saved in xxx_files/sheet001.htm, the url used in the main html file should be like "src="xxx_files/sheet001.htm""
```csharp
public string DefaultPath { get; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StreamProviderOptionsPropertyDefaultPathDemo
{
public static void Run()
{
// Create a new Workbook
Workbook workbook = new Workbook();
// Create StreamProviderOptions with ResourceLoadingType and DefaultPath
StreamProviderOptions options = new StreamProviderOptions(ResourceLoadingType.Default, "1.DefaultPathExample");
// Demonstrate DefaultPath usage
Console.WriteLine("StreamProviderOptions DefaultPath: " + options.DefaultPath);
// Example of using the options with a stream (simplified demonstration)
using (MemoryStream stream = new MemoryStream())
{
options.Stream = stream;
if (options.DefaultPath.IndexOf("1.") >= 0)
{
Console.WriteLine("Processing stream for path: " + options.DefaultPath);
// Perform operations with the stream
workbook.Save(stream, SaveFormat.Xlsx);
}
}
}
}
}
```
### See Also
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
