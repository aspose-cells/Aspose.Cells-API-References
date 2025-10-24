##IStreamProvider.CloseStream
IStreamProvider method. Closes the stream
## IStreamProvider.CloseStream method
Closes the stream.
```csharp
public void CloseStream(StreamProviderOptions options)
```
| Parameter | Type | Description |
| --- | --- | --- |
| options | StreamProviderOptions |  |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo : IStreamProvider
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of the demo class implementing IStreamProvider
var streamProvider = new IStreamProviderMethodCloseStreamWithStreamProviderOptionsDemo();
// Create StreamProviderOptions
var options = new StreamProviderOptions
{
ResourceLoadingType = ResourceLoadingType.Default,
CustomPath = "output_files/sheet001.htm",
Stream = new MemoryStream()
};
try
{
// Call the CloseStream method
streamProvider.CloseStream(options);
Console.WriteLine("CloseStream method executed successfully with StreamProviderOptions");
// Demonstrate effect - in real scenario, this would close the stream
Console.WriteLine($"Stream closed status: {options.Stream == null}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing CloseStream method: {ex.Message}");
}
// Save the workbook
workbook.Save("IStreamProviderCloseStreamDemo.xlsx");
}
public void InitStream(StreamProviderOptions options)
{
// Implementation required by interface
}
public void CloseStream(StreamProviderOptions options)
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
* class [StreamProviderOptions](../../streamprovideroptions/)
* interface [IStreamProvider](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
