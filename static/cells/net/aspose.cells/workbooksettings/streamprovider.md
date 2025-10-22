##WorkbookSettings.StreamProvider
WorkbookSettings property. Gets and sets the stream provider for external resource
## WorkbookSettings.StreamProvider property
Gets and sets the stream provider for external resource.
```csharp
[Obsolete("Use ResourceProvider property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public IStreamProvider StreamProvider { get; set; }
```
### Remarks
NOTE: This member is now obsolete. Instead, please use ResourceProvider property. This property will be removed 12 months later since June 2022. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class CustomStreamProvider1 : IStreamProvider
{
private MemoryStream stream;
public void InitStream(StreamProviderOptions options)
{
stream = new MemoryStream();
options.Stream = stream;
}
public void CloseStream(StreamProviderOptions options)
{
stream.Close();
Console.WriteLine($"Stream closed. Content length: {stream.Length} bytes");
}
}
public class WorkbookSettingsPropertyStreamProviderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Access workbook settings
WorkbookSettings settings = workbook.Settings;
// Display current StreamProvider value
Console.WriteLine("Current StreamProvider value: " + (settings.StreamProvider == null ? "null" : "custom provider"));
// Set a custom stream provider
settings.StreamProvider = new CustomStreamProvider1();
// Add some data to demonstrate stream usage
worksheet.Cells["A1"].PutValue("Test data for stream provider");
// Save the workbook - this will trigger the stream provider
workbook.Save("PropertyStreamProviderDemo.xlsx");
// Reset the stream provider
settings.StreamProvider = null;
Console.WriteLine("StreamProvider reset to null");
}
}
}
```
### See Also
* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
