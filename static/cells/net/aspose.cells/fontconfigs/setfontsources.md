##FontConfigs.SetFontSources
FontConfigs method. Sets the fonts sources
## FontConfigs.SetFontSources method
Sets the fonts sources.
```csharp
public static void SetFontSources(FontSourceBase[] sources)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sources | FontSourceBase[] | An array of sources that contain TrueType fonts. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.IO;
public class FontConfigsMethodSetFontSourcesWithFontSourceBaseDemo
{
public static void Run()
{
// Create a temporary font file for demonstration
string tempFontFile = Path.Combine(Path.GetTempPath(), "testfont.ttf");
try
{
File.WriteAllBytes(tempFontFile, new byte[0]); // Empty file for demo
// Create font sources
FontSourceBase[] fontSources = new FontSourceBase[]
{
new FolderFontSource(Path.GetTempPath(), true),
new FileFontSource(tempFontFile)
};
try
{
// Call SetFontSources method
FontConfigs.SetFontSources(fontSources);
// Verify the font sources were set
FontSourceBase[] currentSources = FontConfigs.GetFontSources();
Console.WriteLine($"Font sources set successfully. Count: {currentSources.Length}");
// Demonstrate effect by checking if a font is available
bool isAvailable = FontConfigs.IsFontAvailable("Arial");
Console.WriteLine($"Is Arial available: {isAvailable}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing SetFontSources method: {ex.Message}");
}
}
finally
{
// Clean up
if (File.Exists(tempFontFile))
{
File.Delete(tempFontFile);
}
}
}
}
}
```
### See Also
* class [FontSourceBase](../../fontsourcebase/)
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
