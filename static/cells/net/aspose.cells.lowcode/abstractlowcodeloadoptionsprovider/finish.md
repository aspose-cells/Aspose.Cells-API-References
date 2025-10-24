##AbstractLowCodeLoadOptionsProvider.Finish
AbstractLowCodeLoadOptionsProvider method. Releases resources after processing currently part of input
## AbstractLowCodeLoadOptionsProvider.Finish method
Releases resources after processing currently part of input.
```csharp
public virtual void Finish(LowCodeLoadOptions part)
```
| Parameter | Type | Description |
| --- | --- | --- |
| part | LowCodeLoadOptions | the load options used for currently split part. |
### Remarks
By default this method just closes the stream specified by the [`InputStream`](../../lowcodeloadoptions/inputstream/) directly(if the load options specified a Stream as source). User may overwrite this method to control how to release resources according to their requirement and the implementation of [`Current`](../current/).
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
using System.Collections;
public class AbstractLowCodeLoadOptionsProviderMethodFinishWithLowCodeLoadOptionsDemo
{
public static void Run()
{
string[] files = { "file1.xlsx", "file2.xlsx", "file3.xlsx" };
CustomLoadOptionsProvider provider = new CustomLoadOptionsProvider(files);
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
saveOptions.OutputFile = "result.xlsx";
saveOptions.SaveFormat = SaveFormat.Xlsx;
LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
mergeOptions.LoadOptionsProvider = provider;
mergeOptions.SaveOptions = saveOptions;
SpreadsheetMerger.Process(mergeOptions);
}
}
public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
{
public IEnumerator fileIter;
public CustomLoadOptionsProvider(string[] files)
{
fileIter = files.GetEnumerator();
current = new LowCodeLoadOptions();
}
private LowCodeLoadOptions current;
public override LowCodeLoadOptions Current => current;
public override bool MoveNext()
{
if (fileIter.MoveNext())
{
current = new LowCodeLoadOptions();
current.InputFile = fileIter.Current.ToString();
return true;
}
return false;
}
public override void Finish(LowCodeLoadOptions part)
{
base.Finish(part);
}
}
}
```
### See Also
* class [LowCodeLoadOptions](../../lowcodeloadoptions/)
* class [AbstractLowCodeLoadOptionsProvider](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
