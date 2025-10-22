##MemoryFontSource.FontData
MemoryFontSource property. Binary font data
## MemoryFontSource.FontData property
Binary font data.
```csharp
public byte[] FontData { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class MemoryFontSourcePropertyFontDataDemo
{
public static void Run()
{
// Load a TrueType font file into memory
byte[] fontBytes = File.ReadAllBytes("arial.ttf");
// Create a MemoryFontSource instance with the font data
MemoryFontSource memoryFontSource = new MemoryFontSource(fontBytes);
// Display the current FontData value (first 10 bytes for demonstration)
Console.WriteLine("FontData length: " + memoryFontSource.FontData.Length);
Console.Write("First 10 bytes: ");
for (int i = 0; i < 10 && i < memoryFontSource.FontData.Length; i++)
{
Console.Write(memoryFontSource.FontData[i].ToString("X2") + " ");
}
Console.WriteLine();
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create font settings and add our memory font source
FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });
// Apply the font configurations globally (not workbook-specific)
FontConfigs.DefaultFontName = "Arial";
FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });
// Create a style with the custom font
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
// Apply the style to a cell
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["A1"].PutValue("Text using memory font source");
// Save the workbook
workbook.Save("MemoryFontSourceDemo.xlsx");
}
}
}
```
### See Also
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
