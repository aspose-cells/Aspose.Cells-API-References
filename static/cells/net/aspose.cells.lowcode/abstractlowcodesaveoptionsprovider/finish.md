##AbstractLowCodeSaveOptionsProvider.Finish
AbstractLowCodeSaveOptionsProvider method. Releases resources after processing currently split part
## AbstractLowCodeSaveOptionsProvider.Finish method
Releases resources after processing currently split part.
```csharp
public virtual void Finish(LowCodeSaveOptions part)
```
| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeSaveOptions | the save options used for currently split part. |
### Remarks
By default this method just closes the stream specified by the [`OutputStream`](../../lowcodesaveoptions/outputstream/) directly(if the save options specified a Stream as destination). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`GetSaveOptions`](../getsaveoptions/).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo
{
public static void Run()
{
LowCodeLoadOptions loadOptions = new LowCodeLoadOptions();
loadOptions.InputFile = "split.xlsx";
// Create concrete provider instance
var provider = new CustomLowCodeSaveOptionsProvider();
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
splitOptions.SaveOptionsProvider = provider;
splitOptions.LoadOptions = loadOptions;
SpreadsheetSplitter.Process(splitOptions);
}
}
// Concrete implementation of AbstractLowCodeSaveOptionsProvider
public class CustomLowCodeSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override void Finish(LowCodeSaveOptions part)
{
base.Finish(part);
}
// Implement the required abstract method
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
{
if (partInfo == null)
{
throw new ArgumentNullException(nameof(partInfo));
}
LowCodeSaveOptions result = new LowCodeSaveOptions();
result.SaveFormat = SaveFormat.Xlsx;
result.OutputFile = partInfo.SheetName + "_split.xlsx";
Console.WriteLine(result.OutputFile);
return result;
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [AbstractLowCodeSaveOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
