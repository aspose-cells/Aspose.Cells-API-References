##IStreamProvider.InitStream
IStreamProvider method. Gets the stream
## IStreamProvider.InitStream method
Gets the stream.
```csharp
public void InitStream(StreamProviderOptions options)
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
public class IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo : IStreamProvider
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of the demo class implementing IStreamProvider
var streamProvider = new IStreamProviderMethodInitStreamWithStreamProviderOptionsDemo();
// Prepare StreamProviderOptions
StreamProviderOptions options = new StreamProviderOptions
{
ResourceLoadingType = ResourceLoadingType.Default,
CustomPath = "custom_path",
Stream = new MemoryStream()
};
try
{
// Call the InitStream method with StreamProviderOptions parameter
streamProvider.InitStream(options);
Console.WriteLine("InitStream method executed successfully with StreamProviderOptions parameter");
// Demonstrate effect - in this case we're just showing the stream is initialized
Console.WriteLine($"Stream initialized: {options.Stream != null}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing InitStream method: {ex.Message}");
}
// Save the result
workbook.Save("MethodInitStreamWithStreamProviderOptionsDemo.xlsx");
}
public void InitStream(StreamProviderOptions options)
{
// Implementation of InitStream
Console.WriteLine($"Initializing stream with ResourceLoadingType: {options.ResourceLoadingType}");
}
public void CloseStream(StreamProviderOptions options)
{
// Implementation of CloseStream
if (options.Stream != null)
{
options.Stream.Close();
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
