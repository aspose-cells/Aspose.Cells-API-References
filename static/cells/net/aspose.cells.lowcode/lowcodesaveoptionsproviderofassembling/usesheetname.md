##LowCodeSaveOptionsProviderOfAssembling.UseSheetName
LowCodeSaveOptionsProviderOfAssembling property. Whether builds the file path with sheet name instead of sheet index. Default value is false
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property
Whether builds the file path with sheet name instead of sheet index. Default value is false.
```csharp
public bool UseSheetName { get; set; }
```
### Remarks
The sheet name will never be rebuilt automatically. So when set it to true, please make sure there is no special sheet name that can cause invalid file path or name.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
{
public static void Run()
{
// Create a new workbook with named worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "MonthlyReport";
// Add sample data for splitting demonstration
for(int i = 0; i < 15; i++)
{
worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
}
// Create and configure the provider
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "split_files/",
PathTail = ".xlsx",
SheetPrefix = "Sheet_",
SplitPartPrefix = "Part_",
SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
};
// Demonstrate UseSheetName=false (default)
Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);
// Change property and demonstrate new behavior
provider.UseSheetName = true;
Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);
Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
}
}
}
```
### See Also
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
