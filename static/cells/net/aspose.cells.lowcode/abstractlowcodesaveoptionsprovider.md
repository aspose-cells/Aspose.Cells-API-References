##Class AbstractLowCodeSaveOptionsProvider
Aspose.Cells.LowCode.AbstractLowCodeSaveOptionsProvider class. Implementation to provide multiple save options for processes that require multiple outputs. For example SpreadsheetSplitter feature requires multiple destinations to save the split files
## AbstractLowCodeSaveOptionsProvider class
Implementation to provide multiple save options for processes that require multiple outputs. For example, [`SpreadsheetSplitter`](../spreadsheetsplitter/) feature requires multiple destinations to save the split files.
```csharp
public abstract class AbstractLowCodeSaveOptionsProvider
```
## Methods
| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Releases resources after processing currently split part. |
| abstract [GetSaveOptions](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/getsaveoptions/)(SplitPartInfo) | Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassAbstractLowCodeSaveOptionsProviderDemo
{
public static void Run()
{
// Create a custom provider by extending AbstractLowCodeSaveOptionsProvider
var customProvider = new CustomSaveOptionsProvider();
// Create a workbook and worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some data
worksheet.Cells["A1"].PutValue("Test Data");
// Create split part info - in real usage, this would come from the API
// Since we can't construct it directly, we'll just pass null for demonstration
SplitPartInfo splitPartInfo = null;
// Get save options from provider
LowCodeSaveOptions saveOptions = customProvider.GetSaveOptions(splitPartInfo);
// Configure save options (example)
saveOptions.SaveFormat = SaveFormat.Xlsx;
// Demonstrate finishing the process
customProvider.Finish(saveOptions);
// Save the workbook (not directly related to provider, just for demo)
workbook.Save("LowCodeSaveOptionsDemo.xlsx");
}
}
// Custom implementation of AbstractLowCodeSaveOptionsProvider
public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
{
// Create and return custom save options based on part info
return new LowCodeSaveOptions()
{
SaveFormat = SaveFormat.Xlsx
// Removed CachedFileFolder as it doesn't exist in LowCodeSaveOptions
};
}
public override void Finish(LowCodeSaveOptions part)
{
// Cleanup or finalization logic here
Console.WriteLine("Save operation completed for part");
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
