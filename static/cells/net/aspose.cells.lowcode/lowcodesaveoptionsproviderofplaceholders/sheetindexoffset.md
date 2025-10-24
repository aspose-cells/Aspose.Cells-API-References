##LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset
LowCodeSaveOptionsProviderOfPlaceHolders property. Offset of sheets index between what used in file path and its actual valueSheetIndex
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property
Offset of sheet's index between what used in file path and its actual value([`SheetIndex`](../../splitpartinfo/sheetindex/)).
```csharp
public int SheetIndexOffset { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexOffsetDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
// Create an instance of LowCodeSaveOptionsProviderOfPlaceHolders
string pathTemplate = "output_{sheet_index}.xlsx";
var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);
// Display current SheetIndexOffset value (default is 0)
Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);
// Set SheetIndexOffset to 1 to shift sheet indices in output filenames
optionsProvider.SheetIndexOffset = 1;
Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);
// Configure save options
optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;
// Demonstrate the effect of SheetIndexOffset on output filenames
// Normally this would be used with GetSaveOptions() during actual save operations
Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");
// Reset to default value
optionsProvider.SheetIndexOffset = 0;
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
