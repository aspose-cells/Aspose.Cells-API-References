##FontConfigs.SetFontFolders
FontConfigs method. Sets the fonts folders
## FontConfigs.SetFontFolders method
Sets the fonts folders
```csharp
public static void SetFontFolders(string[] fontFolders, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolders | String[] | The folders that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class FontConfigsMethodSetFontFoldersWithStringBooleanDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set some text that will use custom fonts
worksheet.Cells["A1"].PutValue("Text with custom font");
// Prepare font folders (replace with actual paths on your system)
string[] fontFolders = new string[]
{
@"C:\Windows\Fonts",
@"D:\CustomFonts"
};
bool recursiveSearch = true;
try
{
// Call SetFontFolders method with String[] and Boolean parameters
FontConfigs.SetFontFolders(fontFolders, recursiveSearch);
// Apply a font that might be in one of these folders
Style style = worksheet.Cells["A1"].GetStyle();
style.Font.Name = "SomeCustomFont"; // Replace with actual font name
worksheet.Cells["A1"].SetStyle(style);
Console.WriteLine("Font folders set successfully. Workbook may use fonts from these locations.");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting font folders: {ex.Message}");
}
// Save the workbook
workbook.Save("FontConfigsSetFontFoldersDemo.xlsx");
}
}
}
```
### See Also
* class [FontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
