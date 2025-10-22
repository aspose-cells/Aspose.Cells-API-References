##LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix
LowCodeSaveOptionsProviderOfPlaceHolders property. Prefix for the index of worksheet
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property
Prefix for the index of worksheet.
```csharp
public string SheetNamePrefix { get; set; }
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
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets[0].Name = "SalesData";
workbook.Worksheets.Add("FinancialReport");
// Initialize provider with path template containing sheet placeholder
string pathTemplate = "output_{sheet}.xlsx";
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);
// Display initial SheetNamePrefix value (empty by default)
Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);
// Set new prefix and ensure path generation includes sheet info
provider.SheetNamePrefix = "Q4_";
provider.BuildPathWithSheetAlways = true;
// Configure save options with correct format
provider.SaveOptionsTemplate = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Xlsx // Set the correct save format
};
// Save workbook using provider - generates "output_Q4_SalesData.xlsx" and "output_Q4_FinancialReport.xlsx"
workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
