##FontConfigs.GetFontSources
FontConfigs method. Gets a copy of the array that contains the list of sources
## FontConfigs.GetFontSources method
Gets a copy of the array that contains the list of sources
```csharp
public static FontSourceBase[] GetFontSources()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsMethodGetFontSourcesDemo
{
public static void Run()
{
try
{
// Get the current font sources
FontSourceBase[] fontSources = FontConfigs.GetFontSources();
// Display information about each font source
if (fontSources != null)
{
Console.WriteLine("Current font sources:");
foreach (var source in fontSources)
{
Console.WriteLine($"Type: {source.GetType().Name}");
if (source is FolderFontSource folderSource)
{
Console.WriteLine($"Folder path: {folderSource.FolderPath}");
Console.WriteLine($"Scan subfolders: {folderSource.ScanSubFolders}");
}
else if (source is FileFontSource fileSource)
{
Console.WriteLine($"File path: {fileSource.FilePath}");
}
else if (source is MemoryFontSource memorySource)
{
Console.WriteLine($"Font data present: {memorySource.FontData != null}");
}
Console.WriteLine();
}
}
else
{
Console.WriteLine("No font sources are currently set.");
}
// Create a new workbook to demonstrate the effect
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some text with a font that might use these sources
worksheet.Cells["A1"].PutValue("Font Sources Demo");
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Name = "Arial";
style.Font.Size = 14;
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("FontConfigsGetFontSourcesDemo.xlsx");
Console.WriteLine("Workbook saved successfully.");
}
catch (Exception ex)
{
Console.WriteLine($"Error while working with font sources: {ex.Message}");
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
