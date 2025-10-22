##LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways
LowCodeSaveOptionsProviderOfAssembling property. Whether add split part index to file path always. Default value is false that is when there is only one split part the split part index and corresponding prefix will not be added to the file path
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSplitPartAlways property
Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path.
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
public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSplitPartAlwaysDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 20; i++)
{
worksheet.Cells[i, 0].Value = "Data Row " + (i + 1);
}
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "SplitData/",
PathTail = ".xlsx",
SplitPartPrefix = "Part_",
SaveOptionsTemplate = new LowCodeSaveOptions()
};
Console.WriteLine("Initial BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
workbook.Save("Output1", provider.SaveOptionsTemplate.SaveFormat);
provider.BuildPathWithSplitPartAlways = true;
Console.WriteLine("Updated BuildPathWithSplitPartAlways: " + provider.BuildPathWithSplitPartAlways);
workbook.Save("Output2", provider.SaveOptionsTemplate.SaveFormat);
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
