##AbstractTextLoadOptions.Encoding
AbstractTextLoadOptions property. Gets and sets the default encoding. Only applies for csv file
## AbstractTextLoadOptions.Encoding property
Gets and sets the default encoding. Only applies for csv file.
```csharp
public Encoding Encoding { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class AbstractTextLoadOptionsPropertyEncodingDemo
{
public static void Run()
{
// Create sample CSV data in ASCII encoding
MemoryStream ms = new MemoryStream();
byte[] data = Encoding.ASCII.GetBytes("Name,Age\nJohn,30\nJane,25");
ms.Write(data, 0, data.Length);
ms.Seek(0, SeekOrigin.Begin);
// Load workbook with ASCII encoding specified
Workbook wb = new Workbook(ms, new TxtLoadOptions() { Encoding = Encoding.ASCII });
Cells cells = wb.Worksheets[0].Cells;
// Display loaded data
Console.WriteLine($"A1: {cells[0, 0].StringValue}");
Console.WriteLine($"B1: {cells[0, 1].StringValue}");
Console.WriteLine($"A2: {cells[1, 0].StringValue}");
Console.WriteLine($"B2: {cells[1, 1].IntValue}");
// Add some Unicode text
cells[2, 0].PutValue("日本語のテキスト");
// Save with UTF-8 encoding
MemoryStream outputStream = new MemoryStream();
wb.Save(outputStream, new TxtSaveOptions() { Encoding = Encoding.UTF8 });
// Display first few bytes to show UTF-8 BOM
byte[] outputBytes = outputStream.ToArray();
Console.WriteLine($"First 3 bytes: {BitConverter.ToString(outputBytes, 0, 3)}");
}
}
}
```
### See Also
* class [AbstractTextLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
