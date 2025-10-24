##Class MemoryFontSource
Aspose.Cells.MemoryFontSource class. Represents the single TrueType font file stored in memory
## MemoryFontSource class
Represents the single TrueType font file stored in memory.
```csharp
public class MemoryFontSource : FontSourceBase
```
## Constructors
| Name | Description |
| --- | --- |
| [MemoryFontSource](memoryfontsource/)(byte[]) | Ctor. |
## Properties
| Name | Description |
| --- | --- |
| [FontData](../../aspose.cells/memoryfontsource/fontdata/) { get; } | Binary font data. |
| override [Type](../../aspose.cells/memoryfontsource/type/) { get; } | Returns the type of the font source. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class CellsClassMemoryFontSourceDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Load a TrueType font file into memory
byte[] fontData = File.ReadAllBytes("arial.ttf");
// Create an instance of MemoryFontSource with the font data
MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
// Create font sources array containing our memory font source
FontSourceBase[] fontSources = new FontSourceBase[] { memoryFontSource };
// Set the font sources using FontConfigs
FontConfigs.SetFontSources(fontSources);
// Use the custom font in a cell
worksheet.Cells["A1"].PutValue("Text with custom font from memory");
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("MemoryFontSourceDemo.xlsx");
}
}
}
```
### See Also
* class [FontSourceBase](../fontsourcebase/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
