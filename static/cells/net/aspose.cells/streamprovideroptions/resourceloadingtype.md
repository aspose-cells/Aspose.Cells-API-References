##StreamProviderOptions.ResourceLoadingType
StreamProviderOptions property. Gets and sets the type of loading resource
## StreamProviderOptions.ResourceLoadingType property
Gets and sets the type of loading resource.
```csharp
public ResourceLoadingType ResourceLoadingType { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StreamProviderOptionsPropertyResourceLoadingTypeDemo
{
public static void Run()
{
// Create workbook with stream provider options
var options = new StreamProviderOptions
{
ResourceLoadingType = ResourceLoadingType.UserProvided
};
// Demonstrate different resource loading behaviors
if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
{
// Provide a custom memory stream
options.Stream = new MemoryStream();
Console.WriteLine("Using user-provided memory stream");
}
else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
{
// Skip loading by using null stream
options.Stream = Stream.Null;
Console.WriteLine("Skipping resource loading");
}
else
{
// Default file loading behavior
string defaultPath = "default_resource.txt";
options.Stream = new FileStream(defaultPath, FileMode.Open, FileAccess.Read);
Console.WriteLine("Loading resource from default path");
}
// Cleanup
options.Stream?.Dispose();
}
}
}
```
### See Also
* enum [ResourceLoadingType](../../resourceloadingtype/)
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
