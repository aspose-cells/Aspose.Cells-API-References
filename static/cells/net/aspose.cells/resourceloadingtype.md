##Enum ResourceLoadingType
Aspose.Cells.ResourceLoadingType enum. Represents how to loading the linked resource
## ResourceLoadingType enumeration
Represents how to loading the linked resource.
```csharp
public enum ResourceLoadingType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Loads this resource as usual. |
| Skip | `1` | Skips loading of this resource. |
| UserProvided | `2` | Use stream provided by user |
### Examples
```csharp
using Aspose.Cells;
using System;
using System.IO;
namespace AsposeCellsExamples
{
public class ResourceLoadingTypeDemo
{
public static void ResourceLoadingTypeExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a new worksheet to the workbook
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data to the worksheet
worksheet.Cells["A1"].PutValue("Resource");
worksheet.Cells["A2"].PutValue("Default");
worksheet.Cells["A3"].PutValue("Skip");
worksheet.Cells["A4"].PutValue("UserProvided");
// Save the workbook to HTML with custom stream provider
HtmlSaveOptions saveOptions = new HtmlSaveOptions(SaveFormat.Html)
{
StreamProvider = new CustomStreamProvider()
};
workbook.Save("ResourceLoadingTypeExample.html", saveOptions);
}
}
public class CustomStreamProvider : IStreamProvider
{
public void InitStream(StreamProviderOptions options)
{
if (options.ResourceLoadingType == ResourceLoadingType.UserProvided)
{
// Provide a custom stream for the resource
options.Stream = new MemoryStream();
}
else if (options.ResourceLoadingType == ResourceLoadingType.Skip)
{
// Skip loading the resource
options.Stream = Stream.Null;
}
else
{
// Load the resource as usual
options.Stream = new FileStream(options.DefaultPath, FileMode.Open, FileAccess.Read);
}
}
public void CloseStream(StreamProviderOptions options)
{
// Close the stream if it is not null
options.Stream?.Close();
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
