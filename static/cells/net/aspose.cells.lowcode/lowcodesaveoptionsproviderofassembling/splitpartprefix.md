##LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix
LowCodeSaveOptionsProviderOfAssembling property. Prefix for the index of split part
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property
Prefix for the index of split part.
```csharp
public string SplitPartPrefix { get; set; }
```
### Remarks
If there is only one split part and [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) is false, then this prefix and the split part index(0) will not be added to the resultant file path.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
{
public static void Run()
{
// Create workbook with data spanning multiple pages
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 100; i++)
worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";
// Configure page settings to create multiple pages
worksheet.PageSetup.PrintArea = "A1:A30";
worksheet.PageSetup.FitToPagesTall = 1;
// Initialize save options provider with split configuration
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "SplitResults/",
SplitPartPrefix = "OriginalPart_",
PathTail = ".pdf",
SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
};
Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
// Save with initial prefix (will generate SplitResults/OriginalPart_0.pdf etc.)
workbook.Save("InitialSplit.pdf", new PdfSaveOptions());
// Modify split prefix
provider.SplitPartPrefix = "ModifiedPart_";
Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");
// Save with modified prefix (will generate SplitResults/ModifiedPart_0.pdf etc.)
workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
