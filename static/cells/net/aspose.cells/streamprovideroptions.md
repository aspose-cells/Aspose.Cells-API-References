##Class StreamProviderOptions
Aspose.Cells.StreamProviderOptions class. Represents the stream options
## StreamProviderOptions class
Represents the stream options.
```csharp
public class StreamProviderOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Initializes a new instance of the `StreamProviderOptions` class. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Initializes a new instance of the `StreamProviderOptions` class. |
## Properties
| Name | Description |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | The default path(URL) saved in generated html file for the referred source. For example, the sheet data saved in xxx_files/sheet001.htm, the url used in the main html file should be like "src="xxx_files/sheet001.htm"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Gets and sets the type of loading resource. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Gets/Sets the stream |
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassStreamProviderOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create StreamProviderOptions
StreamProviderOptions options = new StreamProviderOptions();
// Set a memory stream for demonstration
options.Stream = new MemoryStream();
// Use the stream (example: save workbook to the stream)
workbook.Save(options.Stream, SaveFormat.Xlsx);
// Demonstrate closing the stream
CloseStream(options);
}
public static void CloseStream(StreamProviderOptions options)
{
if (options.Stream != null)
{
options.Stream.Close();
options.Stream = null;
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
