##AbstractLowCodeSaveOptionsProvider.GetSaveOptions
AbstractLowCodeSaveOptionsProvider method. Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part
## AbstractLowCodeSaveOptionsProvider.GetSaveOptions method
Gets the save options from which to get the output settings for currently split part. Returning null denotes to skip given part.
```csharp
public abstract LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
using System;
public class AbstractLowCodeSaveOptionsProviderMethodGetSaveOptionsWithSplitPartInfoDemo
{
public static void Run()
{
LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
loadOptions.InputFile = "split.xlsx";
// Create concrete provider instance
var provider = new CustomSaveOptionsProvider();
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
splitOptions.SaveOptionsProvider = provider;
splitOptions.LoadOptions = loadOptions;
SpreadsheetSplitter.Process(splitOptions);
}
}
// Custom implementation of AbstractLowCodeSaveOptionsProvider
public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
{
if (partInfo == null)
{
throw new ArgumentNullException(nameof(partInfo));
}
// Create custom save options based on part info
LowCodeSaveOptions result = new LowCodeSaveOptions();
result.SaveFormat = SaveFormat.Xlsx;
result.OutputFile = $"Part_{partInfo.PartIndex}_Sheet_{partInfo.SheetName}.xlsx";
Console.WriteLine(result.OutputFile);
return result;
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [SplitPartInfo](../../splitpartinfo/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
