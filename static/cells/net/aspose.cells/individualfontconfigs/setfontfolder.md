##IndividualFontConfigs.SetFontFolder
IndividualFontConfigs method. Sets the fonts folder
## IndividualFontConfigs.SetFontFolder method
Sets the fonts folder
```csharp
public void SetFontFolder(string fontFolder, bool recursive)
```
| Parameter | Type | Description |
| --- | --- | --- |
| fontFolder | String | The folder that contains TrueType fonts. |
| recursive | Boolean | Determines whether or not to scan subfolders. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class IndividualFontConfigsMethodSetFontFolderWithStringBooleanDemo
{
public static void Run()
{
// Create an instance of IndividualFontConfigs
IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
// Specify the font folder path and whether to search recursively
string fontFolderPath = @"C:\Windows\Fonts";
bool recursiveSearch = true;
try
{
// Call SetFontFolder with the specified parameters
fontConfigs.SetFontFolder(fontFolderPath, recursiveSearch);
Console.WriteLine($"Successfully set font folder to: {fontFolderPath}");
Console.WriteLine($"Recursive search enabled: {recursiveSearch}");
// Create a workbook to demonstrate font usage
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set a style that might use fonts from the specified folder
Style style = workbook.CreateStyle();
style.Font.Name = "Arial"; // Assuming Arial exists in the font folder
style.Font.Size = 12;
worksheet.Cells["A1"].Value = "Text with font from specified folder";
worksheet.Cells["A1"].SetStyle(style);
// Save the workbook
workbook.Save("FontConfigDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error setting font folder: {ex.Message}");
}
}
}
}
```
### See Also
* class [IndividualFontConfigs](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
