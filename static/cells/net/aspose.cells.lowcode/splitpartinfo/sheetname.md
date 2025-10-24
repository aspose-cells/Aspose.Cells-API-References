##SplitPartInfo.SheetName
SplitPartInfo property. Name of the sheet where current part is in
## SplitPartInfo.SheetName property
Name of the sheet where current part is in.
```csharp
public string SheetName { get; }
```
### Remarks
May be null for some situations, such as when rendering the whole workbook to tiff image.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using AsposeCellsExamples.AbstractLowCodeSaveOptionsProviderMethodFinishWithLowCodeSaveOptionsDemo;
using System;
using System.Reflection;
public class SplitPartInfoPropertySheetNameDemo
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
* class [SplitPartInfo](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
