##Class FontConfigs
Aspose.Cells.FontConfigs class. Specifies font settings
## FontConfigs class
Specifies font settings
```csharp
public class FontConfigs
```
## Constructors
| Name | Description |
| --- | --- |
| [FontConfigs](fontconfigs/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| static [DefaultFontName](../../aspose.cells/fontconfigs/defaultfontname/) { get; set; } | Gets or sets the default font name. |
| static [PreferSystemFontSubstitutes](../../aspose.cells/fontconfigs/prefersystemfontsubstitutes/) { get; set; } | Indicate whether to use system font substitutes first or not when a font is not presented and the substitute of this font is not set. e.g. On Ubuntu, "Arial" font is generally substituted by "Liberation Sans". Default value is false. |
## Methods
| Name | Description |
| --- | --- |
| static [GetFontFileDataInfo](../../aspose.cells/fontconfigs/getfontfiledatainfo/)(string, bool, bool, bool) | Get data infomation of font file data. |
| static [GetFontSources](../../aspose.cells/fontconfigs/getfontsources/)() | Gets a copy of the array that contains the list of sources |
| static [GetFontSubstitutes](../../aspose.cells/fontconfigs/getfontsubstitutes/)(string) | Returns array containing font substitute names to be used if original font is not presented. |
| static [IsFontAvailable](../../aspose.cells/fontconfigs/isfontavailable/)(string) | Indicate whether the font is available. |
| static [SetFontFolder](../../aspose.cells/fontconfigs/setfontfolder/)(string, bool) | Sets the fonts folder |
| static [SetFontFolders](../../aspose.cells/fontconfigs/setfontfolders/)(string[], bool) | Sets the fonts folders |
| static [SetFontSources](../../aspose.cells/fontconfigs/setfontsources/)(FontSourceBase[]) | Sets the fonts sources. |
| static [SetFontSubstitutes](../../aspose.cells/fontconfigs/setfontsubstitutes/)(string, string[]) | Font substitute names for given original font name. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassFontConfigsDemo
{
public static void Run()
{
// Set custom font folder
string fontFolder = @"C:\MyFonts\";
FontConfigs.SetFontFolder(fontFolder, true);
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Set sample text with different fonts
worksheet.Cells["A1"].PutValue("Text with default font");
worksheet.Cells["A2"].PutValue("Text with custom font");
// Apply custom font style
Style style = workbook.CreateStyle();
style.Font.Name = "MyCustomFont"; // This font should exist in the custom font folder
worksheet.Cells["A2"].SetStyle(style);
// Save to HTML to demonstrate font rendering
HtmlSaveOptions options = new HtmlSaveOptions
{
ExportImagesAsBase64 = true,
PresentationPreference = true
};
workbook.Save("output.html", options);
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
