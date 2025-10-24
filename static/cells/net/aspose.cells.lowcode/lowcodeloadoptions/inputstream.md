##LowCodeLoadOptions.InputStream
LowCodeLoadOptions property. Gets and sets the Stream of the template
## LowCodeLoadOptions.InputStream property
Gets and sets the Stream of the template.
```csharp
public Stream InputStream { get; set; }
```
### Remarks
When setting a non-null Stream to this property, the previously set value for [`InputFile`](../inputfile/) will be ignored.
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.LowCode;
namespace AsposeCellsExamples
{
public class LowCodeLoadOptionsPropertyInputStreamDemo
{
public static void Run()
{
// Create sample data in memory stream
byte[] data = { 0x48, 0x65, 0x6C, 0x6C, 0x6F }; // "Hello" in bytes
using (MemoryStream stream = new MemoryStream(data))
{
// Create load options with InputStream
var loadOptions = new LowCodeLoadOptions() { InputStream = stream };
// Create a new workbook using the stream
using (Workbook workbook = new Workbook(stream))
{
// Access the first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate the content was loaded
Console.WriteLine("First cell value: " + worksheet.Cells["A1"].Value);
}
}
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
