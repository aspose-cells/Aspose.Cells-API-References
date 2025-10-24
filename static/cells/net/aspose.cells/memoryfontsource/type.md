##MemoryFontSource.Type
MemoryFontSource property. Returns the type of the font source
## MemoryFontSource.Type property
Returns the type of the font source.
```csharp
public override FontSourceType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class MemoryFontSourcePropertyTypeDemo
{
public static void Run()
{
// Load a TrueType font file into memory
byte[] fontData = File.ReadAllBytes("arial.ttf");
// Create a MemoryFontSource instance with the font data
MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
// Display the current Type value
Console.WriteLine("MemoryFontSource Type: " + memoryFontSource.Type);
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set font sources using FontConfigs
FontConfigs.SetFontSources(new FontSourceBase[] { memoryFontSource });
// Verify the font source type is MemoryFont
if (memoryFontSource.Type == FontSourceType.MemoryFont)
{
// Use the font in a cell
Style style = workbook.CreateStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["A1"].PutValue("Text using memory font source");
// Add information about the font source type
worksheet.Cells["A2"].PutValue("Font source type: " + memoryFontSource.Type);
}
// Save the workbook
workbook.Save("MemoryFontSourceTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FontSourceType](../../fontsourcetype/)
* class [MemoryFontSource](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
