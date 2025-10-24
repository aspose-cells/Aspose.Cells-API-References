##Class IndividualFontConfigs
Aspose.Cells.IndividualFontConfigs class. Font configs for each Workbook object
## IndividualFontConfigs class
Font configs for each [`Workbook`](../workbook/) object.
```csharp
public class IndividualFontConfigs
```
## Constructors
| Name | Description |
| --- | --- |
| [IndividualFontConfigs](individualfontconfigs/)() | Ctor. |
## Methods
| Name | Description |
| --- | --- |
| [GetFontSources](../../aspose.cells/individualfontconfigs/getfontsources/)() | Gets a copy of the array that contains the list of sources |
| [GetFontSubstitutes](../../aspose.cells/individualfontconfigs/getfontsubstitutes/)(string) | Returns array containing font substitute names to be used if original font is not presented. |
| [SetFontFolder](../../aspose.cells/individualfontconfigs/setfontfolder/)(string, bool) | Sets the fonts folder |
| [SetFontFolders](../../aspose.cells/individualfontconfigs/setfontfolders/)(string[], bool) | Sets the fonts folders |
| [SetFontSources](../../aspose.cells/individualfontconfigs/setfontsources/)(FontSourceBase[]) | Sets the fonts sources. |
| [SetFontSubstitutes](../../aspose.cells/individualfontconfigs/setfontsubstitutes/)(string, string[]) | Font substitute names for given original font name. |
### Examples
```csharp
using System;
using System.IO;
using System.Text;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsClassIndividualFontConfigsDemo
{
public static void Run()
{
// Create temporary directories for font sources
string tempFontFolder1 = Path.Combine(Path.GetTempPath(), "FontFolder1_" + Guid.NewGuid().ToString());
string tempFontFolder2 = Path.Combine(Path.GetTempPath(), "FontFolder2_" + Guid.NewGuid().ToString());
Directory.CreateDirectory(tempFontFolder1);
Directory.CreateDirectory(tempFontFolder2);
// Create sample CSV file
string csvFilePath = "sample_data.csv";
File.WriteAllText(csvFilePath, "Name,Age\nJohn,30\nAlice,25", Encoding.UTF8);
try
{
// Initialize font configuration
IndividualFontConfigs fontConfigs = new IndividualFontConfigs();
// Set font substitutes for Arial
fontConfigs.SetFontSubstitutes("Arial", new string[] { "Times New Roman", "Verdana" });
// Configure font directories
fontConfigs.SetFontFolder(tempFontFolder1, false);
fontConfigs.SetFontFolders(new string[] { tempFontFolder1, tempFontFolder2 }, true);
// Configure font sources
FontSourceBase[] fontSources = {
new FolderFontSource(tempFontFolder1, false),
new FolderFontSource(tempFontFolder2, true)
};
fontConfigs.SetFontSources(fontSources);
// Create text loading options with font configurations
TxtLoadOptions loadOptions = new TxtLoadOptions(LoadFormat.Csv)
{
FontConfigs = fontConfigs
};
// Load workbook with configured options
using (Workbook workbook = new Workbook(csvFilePath, loadOptions))
{
// Save as Excel file
workbook.Save("output_with_font_config.xlsx");
}
}
finally
{
// Cleanup temporary resources
if (Directory.Exists(tempFontFolder1)) Directory.Delete(tempFontFolder1, true);
if (Directory.Exists(tempFontFolder2)) Directory.Delete(tempFontFolder2, true);
if (File.Exists(csvFilePath)) File.Delete(csvFilePath);
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
