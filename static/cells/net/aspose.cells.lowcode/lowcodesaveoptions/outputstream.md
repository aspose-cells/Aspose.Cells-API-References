##LowCodeSaveOptions.OutputStream
LowCodeSaveOptions property. Gets and sets the Stream for writing the generated data to. When setting this property with value other than null OutputFile will be ignored
## LowCodeSaveOptions.OutputStream property
Gets and sets the Stream for writing the generated data to. When setting this property with value other than null, [`OutputFile`](../outputfile/) will be ignored.
```csharp
public Stream OutputStream { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.IO;
public class LowCodeSaveOptionsPropertyOutputStreamDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Sample OutputStream Demo");
try
{
// Create LowCodeSaveOptions instance
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
// Create a memory stream for demonstration
using (MemoryStream stream = new MemoryStream())
{
// Set the OutputStream property
saveOptions.OutputStream = stream;
saveOptions.SaveFormat = SaveFormat.Xlsx;
// Save using the options (will write to our memory stream)
workbook.Save(saveOptions.OutputStream, saveOptions.SaveFormat);
// Verify the stream was written to
Console.WriteLine($"OutputStream length: {saveOptions.OutputStream.Length} bytes");
Console.WriteLine("OutputStream position reset to 0 for reading");
saveOptions.OutputStream.Position = 0;
// Create a new workbook from the stream to verify content
Workbook verifyWorkbook = new Workbook(saveOptions.OutputStream);
Console.WriteLine($"Verified worksheet count: {verifyWorkbook.Worksheets.Count}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
