##LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways
LowCodeSaveOptionsProviderOfPlaceHolders property. Whether add sheet index or name to file path always. Default value is false that is when there is only one sheet the sheet index and name and corresponding prefixSheetNamePrefix will not be added to the file path
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([`SheetNamePrefix`](../sheetnameprefix/)) will not be added to the file path.
```csharp
public bool BuildPathWithSheetAlways { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
{
public static void Run()
{
// Create workbook with two sheets to demonstrate path differences
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
// Configure provider with sheet index placeholder
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
{
// Demonstrate sheet index offset (optional)
SheetIndexOffset = 1
};
Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
// Save with sheet index only when multiple sheets (default behavior)
provider.BuildPathWithSheetAlways = false;
SaveWithProvider(workbook, provider, "DefaultBehavior");
// Force sheet index in filenames even for single sheets
provider.BuildPathWithSheetAlways = true;
Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
SaveWithProvider(workbook, provider, "ForcedSheetIndex");
}
private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
{
// Configure save options with JSON format to enable splitting
var saveOptions = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Json
};
// Configure provider with the save options
provider.SaveOptionsTemplate = saveOptions;
// Save with provider-determined paths
Console.WriteLine($"Saving with {saveDescription} - check output files");
workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
