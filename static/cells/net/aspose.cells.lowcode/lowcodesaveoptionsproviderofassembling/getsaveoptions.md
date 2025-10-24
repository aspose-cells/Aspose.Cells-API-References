##LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions
LowCodeSaveOptionsProviderOfAssembling method. Gets the save options from which to get the output settings for currently split part
## LowCodeSaveOptionsProviderOfAssembling.GetSaveOptions method
Gets the save options from which to get the output settings for currently split part.
```csharp
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingMethodGetSaveOptionsWithSplitPartInfoDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Name = "DataSheet";
// Add sample data
worksheet.Cells["A1"].Value = "Sample Data for Split";
try
{
// Create an instance of LowCodeSaveOptionsProviderOfAssembling
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "Output/",
PathTail = ".xlsx",
UseSheetName = true,
SheetPrefix = "Sheet_",
SplitPartPrefix = "Part_",
SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
};
// Create a SplitPartInfo instance using reflection since constructor isn't accessible
var splitPartInfo = (SplitPartInfo)Activator.CreateInstance(typeof(SplitPartInfo), nonPublic: true);
// Call GetSaveOptions with the SplitPartInfo parameter
LowCodeSaveOptions saveOptions = provider.GetSaveOptions(splitPartInfo);
Console.WriteLine("SaveOptions created successfully");
Console.WriteLine($"Output format: {saveOptions.SaveFormat}");
// Save the workbook (in real usage this would use the generated save options)
workbook.Save("GetSaveOptionsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error in GetSaveOptions demo: {ex.Message}");
}
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
