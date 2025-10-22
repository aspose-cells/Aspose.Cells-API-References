##FontFileDataInfo.Data
FontFileDataInfo property. Gets binary data of font file
## FontFileDataInfo.Data property
Gets binary data of font file.
```csharp
public byte[] Data { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class FontFileDataInfoPropertyDataDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Load a font file (replace with actual font file path)
string fontFilePath = "samplefont.ttf";
byte[] fontData = File.ReadAllBytes(fontFilePath);
// Create a FontConfigs instance and add the font
FontConfigs.SetFontFolder(Path.GetDirectoryName(fontFilePath), false);
// In real usage, FontFileDataInfo would be obtained from the library
// For demonstration purposes, we'll just show how you would use it if you had one
FontFileDataInfo fontInfo = null; // Normally obtained from library APIs
// Display information about the font data (if available)
Console.WriteLine("Font data length: " + (fontInfo?.Data != null ? fontInfo.Data.Length.ToString() : "null"));
if (fontInfo != null)
{
Console.WriteLine("Font format type: " + fontInfo.FormatType);
}
// In real usage, the Data property would be used to access the font binary data
// For example, you might save it to a file:
if (fontInfo?.Data != null && fontInfo.Data.Length > 0)
{
File.WriteAllBytes("extracted_font.ttf", fontInfo.Data);
Console.WriteLine("Font data extracted to file.");
}
// Save the workbook (the font would affect rendering if used in cells)
workbook.Save("FontDataDemo.xlsx");
}
}
}
```
### See Also
* class [FontFileDataInfo](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
