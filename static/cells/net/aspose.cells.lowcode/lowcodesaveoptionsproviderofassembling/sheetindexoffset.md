##LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset
LowCodeSaveOptionsProviderOfAssembling property. Offset of sheets index between what used in file path and its actual valueSheetIndex
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property
Offset of sheet's index between what used in file path and its actual value([`SheetIndex`](../../splitpartinfo/sheetindex/)).
```csharp
public int SheetIndexOffset { get; set; }
```
### Remarks
Only takes effect when [`UseSheetName`](../usesheetname/) is false.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
{
public static void Run()
{
// Create a new workbook with multiple sheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("SalesData");
workbook.Worksheets.Add("Inventory");
// Initialize save options provider
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "output/Quarter_",
PathTail = ".xlsx",
SheetPrefix = "Sheet",
SheetIndexOffset = 10,
SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
};
// Display original offset
Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");
// Save with initial offset (sheets will be numbered 10 and 11)
workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);
// Change offset and save again
provider.SheetIndexOffset = 100;
Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
// Save with new offset (sheets will be numbered 100 and 101)
workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
