##MemoryFontSource.MemoryFontSource
MemoryFontSource constructor. Ctor
## MemoryFontSource constructor
Ctor.
```csharp
public MemoryFontSource(byte[] fontData)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontData | Byte[] | Binary font data. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class MemoryFontSourceMethodCtorWithByteArrayDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
try
{
// Load a TrueType font file into byte array
byte[] fontData = File.ReadAllBytes("arial.ttf");
// Call the #ctor method with byte array parameter
MemoryFontSource fontSource = new MemoryFontSource(fontData);
// Set font sources using FontConfigs static class
FontConfigs.SetFontSources(new FontSourceBase[] { fontSource });
// Verify the font source properties
Console.WriteLine($"Font source type: {fontSource.Type}");
Console.WriteLine($"Font data length: {fontSource.FontData.Length} bytes");
// Use the font in a cell
Worksheet worksheet = workbook.Worksheets[0];
var style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
worksheet.Cells["A1"].PutValue("Text with custom font");
worksheet.Cells["A1"].SetStyle(style);
Console.WriteLine("MemoryFontSource constructor executed successfully with byte array parameter");
}
catch (FileNotFoundException ex)
{
Console.WriteLine($"Error: Font file not found. {ex.Message}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing MemoryFontSource constructor: {ex.Message}");
}
// Save the result
workbook.Save("MemoryFontSourceCtorDemo.xlsx");
}
}
}
```
### See Also
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
