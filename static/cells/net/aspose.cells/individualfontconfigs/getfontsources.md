##IndividualFontConfigs.GetFontSources
IndividualFontConfigs method. Gets a copy of the array that contains the list of sources
## IndividualFontConfigs.GetFontSources method
Gets a copy of the array that contains the list of sources
```csharp
public FontSourceBase[] GetFontSources()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IndividualFontConfigsMethodGetFontSourcesDemo
{
public static void Run()
{
// Create individual font configurations
IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
// Set some font sources (folders containing fonts)
string fontFolder1 = @"C:\Windows\Fonts";
string fontFolder2 = @"D:\CustomFonts";
fontConfigs.SetFontFolder(fontFolder1, false);
fontConfigs.SetFontFolder(fontFolder2, true);
try
{
// Get the current font sources
FontSourceBase[] fontSources = fontConfigs.GetFontSources();
Console.WriteLine("Current font sources:");
foreach (var source in fontSources)
{
if (source is FolderFontSource folderSource)
{
Console.WriteLine($"- Folder: {folderSource.FolderPath} (Recursive: {folderSource.ScanSubFolders})");
}
}
// Create a workbook to demonstrate the effect
Workbook workbook = new Workbook(FileFormatType.Xlsx);
// Use the font configurations when creating styles or working with fonts
// (Workbook doesn't have a FontConfigs property, so we remove that line)
Worksheet worksheet = workbook.Worksheets[0];
// Use a custom font that might be in one of the folders
Style style = workbook.CreateStyle();
style.Font.Name = "SomeCustomFont";
worksheet.Cells["A1"].SetStyle(style);
worksheet.Cells["A1"].PutValue("Text with custom font");
Console.WriteLine("Workbook created with custom font configurations.");
workbook.Save("MethodGetFontSourcesDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetFontSources method: {ex.Message}");
}
}
}
}
```
### See Also
* class [FontSourceBase](../../fontsourcebase/)
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
