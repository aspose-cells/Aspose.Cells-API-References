##LowCodeSaveOptionsProviderOfAssembling.SheetPrefix
LowCodeSaveOptionsProviderOfAssembling property. Prefix for the index of worksheet
## LowCodeSaveOptionsProviderOfAssembling.SheetPrefix property
Prefix for the index of worksheet.
```csharp
public string SheetPrefix { get; set; }
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
public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetPrefixDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
workbook.Worksheets.Add("Sheet3");
LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
provider.PathHeader = "output/";
provider.PathTail = ".xlsx";
provider.UseSheetName = false;
Console.WriteLine("Current SheetPrefix: " + provider.SheetPrefix);
provider.SheetPrefix = "Report_";
Console.WriteLine("New SheetPrefix: " + provider.SheetPrefix);
for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
{
string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
Console.WriteLine($"Generated file path: {fileName}");
}
provider.SheetPrefix = "Data_";
Console.WriteLine("Updated SheetPrefix: " + provider.SheetPrefix);
for (int sheetIndex = 0; sheetIndex < workbook.Worksheets.Count; sheetIndex++)
{
string fileName = $"{provider.PathHeader}{provider.SheetPrefix}{sheetIndex}{provider.PathTail}";
Console.WriteLine($"Generated file path: {fileName}");
}
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
