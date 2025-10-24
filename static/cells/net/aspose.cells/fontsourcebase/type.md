##FontSourceBase.Type
FontSourceBase property. Returns the type of the font source
## FontSourceBase.Type property
Returns the type of the font source.
```csharp
public abstract FontSourceType Type { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontSourceBasePropertyTypeDemo
{
public static void Run()
{
// Create a workbook instance
Workbook workbook = new Workbook();
// Create a folder font source
FolderFontSource folderFontSource = new FolderFontSource("C:\\MyFonts", true);
// Display the Type property of the font source
Console.WriteLine("Font source type: " + folderFontSource.Type);
// Create a file font source
FileFontSource fileFontSource = new FileFontSource("arial.ttf");
// Display the Type property of the font source
Console.WriteLine("Font source type: " + fileFontSource.Type);
// Create memory font source (example with byte array)
byte[] fontData = System.IO.File.ReadAllBytes("arial.ttf");
MemoryFontSource memoryFontSource = new MemoryFontSource(fontData);
// Display the Type property of the font source
Console.WriteLine("Font source type: " + memoryFontSource.Type);
// Set font sources using the static method
FontConfigs.SetFontSources(new FontSourceBase[] { folderFontSource, fileFontSource, memoryFontSource });
// Save the workbook
workbook.Save("FontSourceTypeDemo.xlsx");
}
}
}
```
### See Also
* enum [FontSourceType](../../fontsourcetype/)
* class [FontSourceBase](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
