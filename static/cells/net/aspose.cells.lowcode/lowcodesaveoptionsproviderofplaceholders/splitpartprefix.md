##LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix
LowCodeSaveOptionsProviderOfPlaceHolders property. Prefix for the index of split part
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property
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
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 25; i++)
{
worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
}
// Configure save options template
LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
// Initialize provider with split part placeholder
LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
{
SaveOptionsTemplate = saveOptionsTemplate
};
// Display and modify SplitPartPrefix
Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
provider.SplitPartPrefix = "Section";
Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");
// Save workbook with split parts using the provider's save format
workbook.Save("output", saveOptionsTemplate.SaveFormat);
Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
