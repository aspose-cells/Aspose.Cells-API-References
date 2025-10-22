##LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset
LowCodeSaveOptionsProviderOfAssembling property. Offset of split parts index between what used in file path and its actual valuePartIndex
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property
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
public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartIndexOffsetDemo
{
public static void Run()
{
// Create workbook with test data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet to create multiple split parts
for(int i = 0; i < 150; i++)
{
worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
}
// Configure page breaks to split into 3 parts
worksheet.HorizontalPageBreaks.Add(0, 50);
worksheet.HorizontalPageBreaks.Add(0, 100);
// Create provider and configure save options
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "output/Part_",
SplitPartPrefix = "-",
PathTail = ".xlsx",
SplitPartIndexOffset = 10
};
// Show initial configuration
Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
Console.WriteLine("First save operation (offset 10):");
Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");
// Change offset and show new configuration
provider.SplitPartIndexOffset = 0;
Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
Console.WriteLine("Second save operation (offset 0):");
Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");
// Actual save operation would typically be:
// workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
