##LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways
LowCodeSaveOptionsProviderOfAssembling property. Whether add sheet index or name to file path always. Default value is false that is when there is only one sheet the sheet indexor name and corresponding prefix will not be added to the file path
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property
Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path.
```csharp
public bool BuildPathWithSheetAlways { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
{
public static void Run()
{
// Create a new workbook with one worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "DataSheet";
// Create an instance of LowCodeSaveOptionsProviderOfAssembling
LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
// Configure path settings
provider.PathHeader = "output/";
provider.PathTail = ".xlsx";
provider.UseSheetName = true; // Use sheet name instead of index
provider.SheetPrefix = "_Sheet_";
provider.SplitPartPrefix = "_Part_";
// Display initial property value
Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
// Demonstrate file path without BuildPathWithSheetAlways
string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
Console.WriteLine("Generated path (default): " + defaultPath);
// Set BuildPathWithSheetAlways to true
provider.BuildPathWithSheetAlways = true;
Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
// Demonstrate file path with BuildPathWithSheetAlways (even with single sheet)
string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
Console.WriteLine("Generated path (updated): " + updatedPath);
// Save the workbook (split behavior would use the provider's settings in real scenarios)
workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
