##LowCodeMergeOptions.LoadOptionsProvider
LowCodeMergeOptions property. Provider of save options for saving the split parts
## LowCodeMergeOptions.LoadOptionsProvider property
Provider of save options for saving the split parts.
```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```
### Remarks
If this property is specified, [`LoadOptions`](../../../aspose.cells/loadoptions/) takes no effect because the output of every split part will be specified by the provider.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create an instance of LowCodeMergeOptions
LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
// Display the current value of LoadOptionsProvider (should be null initially)
Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));
// Create a custom LoadOptionsProvider implementation
mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
// Demonstrate setting the property
Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));
// Use the merge options with the provider
// This would typically be used with methods that process multiple files
// For demonstration, we'll just check if the provider can move to next
bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);
// Save the workbook
workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
}
private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
{
private int counter = 0;
private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();
public override LowCodeLoadOptions Current => options;
public override bool MoveNext()
{
// Simulate having 3 files to process
if (counter < 3)
{
counter++;
return true;
}
return false;
}
public override void Finish(LowCodeLoadOptions part)
{
// Cleanup or finalization logic would go here
}
}
}
}
```
### See Also
* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
