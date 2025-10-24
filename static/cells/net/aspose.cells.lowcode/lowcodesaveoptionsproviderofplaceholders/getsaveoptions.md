##LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions
LowCodeSaveOptionsProviderOfPlaceHolders method. Gets the save options from which to get the output settings for currently split part
## LowCodeSaveOptionsProviderOfPlaceHolders.GetSaveOptions method
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
public class LowCodeSaveOptionsProviderOfPlaceHoldersMethodGetSaveOptionsWithSplitPartInfoDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a SplitPartInfo instance
// Since SplitPartInfo has no parameterless constructor and properties are read-only,
// we'll need to get an instance from somewhere else in the API or use null if allowed
// For demonstration purposes, we'll pass null (assuming the method accepts it)
SplitPartInfo splitPartInfo = null;
// Create the LowCodeSaveOptionsProviderOfPlaceHolders instance
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output_{sheet}.xlsx")
{
SheetIndexOffset = 0,
SplitPartIndexOffset = 0,
BuildPathWithSheetAlways = false,
BuildPathWithSplitPartAlways = false,
SheetNamePrefix = "sheet_",
SheetIndexPrefix = "sheet_",
SplitPartPrefix = "part_",
SaveOptionsTemplate = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Xlsx
}
};
try
{
// Call the GetSaveOptions method with SplitPartInfo parameter
var saveOptions = provider.GetSaveOptions(splitPartInfo);
Console.WriteLine("GetSaveOptions method executed successfully with SplitPartInfo parameter");
Console.WriteLine($"Output file: {saveOptions.OutputFile}");
Console.WriteLine($"Save format: {saveOptions.SaveFormat}");
}
catch (Exception ex)
{
Console.WriteLine($"Error executing GetSaveOptions method: {ex.Message}");
}
// Save the workbook
workbook.Save("MethodGetSaveOptionsWithSplitPartInfoDemo.xlsx");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
