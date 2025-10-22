##LowCodeMergeOptions.SaveOptions
LowCodeMergeOptions property. Save options for saving the split parts
## LowCodeMergeOptions.SaveOptions property
Save options for saving the split parts.
```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeMergeOptionsPropertySaveOptionsDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Merged Data");
// Initialize merge options
LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
Console.WriteLine("Initial SaveOptions: " + (mergeOptions.SaveOptions?.GetType().Name ?? "null"));
// Configure new save options
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions();
saveOptions.SaveFormat = SaveFormat.Xlsx;
// Set password via workbook settings
workbook.Settings.Password = "Aspose1234!";
mergeOptions.SaveOptions = saveOptions;
// Demonstrate effect by saving with configured options
workbook.Save("MergedWithOptions.xlsx", saveOptions.SaveFormat);
Console.WriteLine("Workbook saved with password-protected SaveOptions.");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
