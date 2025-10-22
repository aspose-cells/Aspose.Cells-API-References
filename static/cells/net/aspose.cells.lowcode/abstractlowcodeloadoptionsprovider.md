##Class AbstractLowCodeLoadOptionsProvider
Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider class. Implementation to provide multiple load options for processes that use multiple inputssuch as template files
## AbstractLowCodeLoadOptionsProvider class
Implementation to provide multiple load options for processes that use multiple inputs(such as template files).
```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```
## Properties
| Name | Description |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | Gets the load options from which to load data of currently processed part. |
## Methods
| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | Releases resources after processing currently part of input. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | Checks whether there is more input. |
### Remarks
For example, [`SpreadsheetMerger`](../spreadsheetmerger/) feature requires multiple template files to merge.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
{
public static void Run()
{
// Create a custom implementation of AbstractLowCodeLoadOptionsProvider
var provider = new CustomLoadOptionsProvider();
// Process multiple inputs using the provider
while (provider.MoveNext())
{
// Get current load options
LowCodeLoadOptions currentOptions = provider.Current;
Console.WriteLine($"Processing with load options: {currentOptions}");
// Create workbook with current options
Workbook workbook = new Workbook(FileFormatType.Xlsx);
Worksheet worksheet = workbook.Worksheets[0];
// Demonstrate usage with workbook
worksheet.Cells["A1"].PutValue("Processed with custom provider");
// Finish processing this part
provider.Finish(currentOptions);
}
}
private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
{
private int currentIndex = 0;
private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
{
new LowCodeLoadOptions(),
new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
new LowCodeLoadOptions() // MemorySetting would be handled separately
};
public override LowCodeLoadOptions Current => optionsList[currentIndex];
public override bool MoveNext()
{
if (currentIndex < optionsList.Length - 1)
{
currentIndex++;
return true;
}
return false;
}
public override void Finish(LowCodeLoadOptions part)
{
// Cleanup or finalization logic for each part
Console.WriteLine($"Finished processing part {currentIndex}");
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
