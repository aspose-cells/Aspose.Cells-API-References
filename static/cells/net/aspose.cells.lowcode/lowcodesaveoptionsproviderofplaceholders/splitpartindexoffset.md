##LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset
LowCodeSaveOptionsProviderOfPlaceHolders property. Offset of split parts index between what used in file path and its actual valuePartIndex
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property
Offset of split part's index between what used in file path and its actual value([`PartIndex`](../../splitpartinfo/partindex/)).
```csharp
public int SplitPartIndexOffset { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartIndexOffsetDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 15; i++)
{
worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
}
// Create low code save options template
LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;
// Initialize provider with path template
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
provider.SaveOptionsTemplate = saveOptionsTemplate;
// Display and modify SplitPartIndexOffset
Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
provider.SplitPartIndexOffset = 1;
// Save workbook to generate split parts with adjusted index
workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);
Console.WriteLine("Generated split parts with offset applied.");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
