##LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix
LowCodeSaveOptionsProviderOfPlaceHolders property. Prefix for the index of worksheet
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property
Prefix for the index of worksheet.
```csharp
public string SheetIndexPrefix { get; set; }
```
### Remarks
If there is only one worksheet and [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) is false, then this prefix and the sheet index(or name) will not be added to the resultant file path.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
{
public static void Run()
{
// Create a new workbook with multiple worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Create an instance of LowCodeSaveOptionsProviderOfPlaceHolders
string pathTemplate = "output_{sheetindex}.xlsx";
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);
// Display and modify SheetIndexPrefix
Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
provider.SheetIndexPrefix = "sheet_";
Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);
// Set other required properties
provider.BuildPathWithSheetAlways = true;
provider.SaveOptionsTemplate = new LowCodeSaveOptions();
// Demonstrate the effect of SheetIndexPrefix on file paths
foreach (Worksheet sheet in workbook.Worksheets)
{
// Since we can't create and populate SplitPartInfo directly,
// we'll just demonstrate the naming pattern without it
Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
}
// Save the workbook to demonstrate the naming pattern
workbook.Save("output_sheet_0.xlsx");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
