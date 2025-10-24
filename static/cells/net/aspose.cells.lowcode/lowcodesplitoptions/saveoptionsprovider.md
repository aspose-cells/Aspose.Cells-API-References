##LowCodeSplitOptions.SaveOptionsProvider
LowCodeSplitOptions property. Provider of save options for saving the split parts
## LowCodeSplitOptions.SaveOptionsProvider property
Provider of save options for saving the split parts.
```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```
### Remarks
If this property is specified, [`SaveOptions`](../saveoptions/) takes no effect because the output of every split part will be specified by the provider.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate some sample data
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("Item1");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["A3"].PutValue("Item2");
worksheet.Cells["B3"].PutValue(200);
// Create LowCodeSplitOptions instance
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
// Display current SaveOptionsProvider value (null by default)
Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
// Create a custom SaveOptionsProvider
splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
// Demonstrate the effect of setting SaveOptionsProvider
// In a real scenario, this would be used when splitting files
Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
// Save the workbook (though splitting isn't demonstrated here)
workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
}
}
// Custom implementation of AbstractLowCodeSaveOptionsProvider
public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
{
// Create custom save options for each split part
LowCodeSaveOptions options = new LowCodeSaveOptions();
options.SaveFormat = SaveFormat.Xlsx;
return options;
}
public override void Finish(LowCodeSaveOptions part)
{
// Perform any cleanup after saving each part
Console.WriteLine("Finished saving part");
}
}
}
```
### See Also
* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
