##Class LowCodeMergeOptions
Aspose.Cells.LowCode.LowCodeMergeOptions class. Options for merging multiple template files into one
## LowCodeMergeOptions class
Options for merging multiple template files into one.
```csharp
public class LowCodeMergeOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | Provider of save options for saving the split parts. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | Save options for saving the split parts. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassLowCodeMergeOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Create and configure LowCodeMergeOptions
LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
// Set save options for output format
mergeOptions.SaveOptions = new LowCodeSaveOptions();
// Assign custom load options provider
mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
// Example integration (hypothetical usage with merge functionality)
// This would typically be called with actual file paths
// Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
// Save the workbook (demonstration purposes)
workbook.Save("LowCodeMergeOptionsDemo.xlsx");
}
}
// Custom provider implementing abstract class
public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
{
public override bool MoveNext()
{
// Minimal implementation to satisfy abstract requirement
return false;
}
public override LowCodeLoadOptions Current
{
get { throw new InvalidOperationException(); }
}
public LoadOptions GetLoadOptions(string fileName)
{
if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
{
return new LoadOptions(LoadFormat.Xlsx);
}
return new LoadOptions();
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
