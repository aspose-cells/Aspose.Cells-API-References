##LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways
LowCodeSaveOptionsProviderOfPlaceHolders property. Whether add split part index to file path always. Default value is false that is when there is only one split part the split part index and corresponding prefixSplitPartPrefix will not be added to the file path
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([`SplitPartPrefix`](../splitpartprefix/)) will not be added to the file path.
```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
{
public static void Run()
{
// Create workbook with data that won't be split into multiple parts
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Single Part Demonstration";
// Create provider with path template and split condition that results in one part
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
{
SaveOptionsTemplate = new LowCodeSaveOptions()
};
// Demonstrate property false state (default)
Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
provider.BuildPathWithSplitPartAlways = false;
// This would generate Result.xlsx when only one part exists
Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
ExecuteDummySave(workbook, "Result.xlsx");
// Toggle property and demonstrate true state
provider.BuildPathWithSplitPartAlways = true;
Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
// This would generate Result_0.xlsx even with single part
ExecuteDummySave(workbook, "Result_0.xlsx");
}
private static void ExecuteDummySave(Workbook workbook, string filename)
{
// In real usage, replace with provider-based save operation
Console.WriteLine($"Simulated save operation -> Filename: {filename}");
workbook.Save(filename, SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
