##StreamProviderOptions.Stream
StreamProviderOptions property. Gets/Sets the stream
## StreamProviderOptions.Stream property
Gets/Sets the stream
```csharp
public Stream Stream { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class StreamProviderOptionsPropertyStreamDemo
{
public static void Run()
{
// Create StreamProviderOptions instance
StreamProviderOptions options = new StreamProviderOptions();
// Case 1: When no default path is set - use MemoryStream
options.Stream = new MemoryStream();
Console.WriteLine("Using MemoryStream: " + (options.Stream is MemoryStream));
// Case 2: Simulate having a default path - use FileStream
string outputDir = "output/";
string defaultPath = "testfile.txt"; // Store path separately since DefaultPath is read-only
string path = outputDir + Path.GetFileName(defaultPath);
Directory.CreateDirectory(Path.GetDirectoryName(path));
options.Stream = File.Create(path);
Console.WriteLine("Using FileStream: " + (options.Stream is FileStream));
// Clean up
options.Stream.Dispose();
if (File.Exists(path))
{
File.Delete(path);
}
}
}
}
```
### See Also
* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
