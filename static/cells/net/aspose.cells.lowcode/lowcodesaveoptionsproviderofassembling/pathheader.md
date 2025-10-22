##LowCodeSaveOptionsProviderOfAssembling.PathHeader
LowCodeSaveOptionsProviderOfAssembling property. Header partbefore added content of sheet and split part of file path
## LowCodeSaveOptionsProviderOfAssembling.PathHeader property
Header part(before added content of sheet and split part) of file path.
```csharp
public string PathHeader { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertyPathHeaderDemo
{
public static void Run()
{
// Create a workbook with data that will be split into multiple parts
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 150; i++)
{
worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
}
// Initialize save options provider with default values
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "output/QuarterlyReport_",
PathTail = ".html",
UseSheetName = true,
SaveOptionsTemplate = new LowCodeSaveOptions() // Changed from HtmlSaveOptions to LowCodeSaveOptions
};
Console.WriteLine($"Initial PathHeader: {provider.PathHeader}");
// Modify path configuration
provider.PathHeader = "output/ModifiedReport_";
provider.SheetPrefix = "Sheet_";
provider.SplitPartPrefix = "Part_";
// Demonstrate effect by saving with current provider configuration
workbook.Save("result.html", SaveFormat.Html); // Changed second parameter to SaveFormat.Html
Console.WriteLine("Check 'output' directory for split files named like 'ModifiedReport_Sheet_0_Part_0.html'");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
