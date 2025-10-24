##Class LowCodeSplitOptions
Aspose.Cells.LowCode.LowCodeSplitOptions class. Options for splitting spreadsheet
## LowCodeSplitOptions class
Options for splitting spreadsheet.
```csharp
public class LowCodeSplitOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | Load options for loading the spreadsheet that will be split. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | Save options for saving the split parts. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | Provider of save options for saving the split parts. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using System;
public class LowCodeClassLowCodeSplitOptionsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet with sample data
worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
// Create an instance of LowCodeSplitOptions
LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
// Configure LoadOptions (example: handle password-protected source)
splitOptions.LoadOptions = new LowCodeLoadOptions();
// Configure SaveOptions (example: set default output format)
splitOptions.SaveOptions = new LowCodeSaveOptions();
// Implement custom SaveOptions provider for dynamic output settings
splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
// Example integration: Split workbook into parts using configured options
// (Assume existence of a method like LowCodeEngine.Split(workbook, splitOptions, "outputDir"))
// LowCodeEngine.Split(workbook, splitOptions, "OutputDirectory");
// Save the original workbook for demonstration
workbook.Save("LowCodeSplitOptionsDemo.xlsx");
}
// Custom SaveOptionsProvider implementation
private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
{
public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
{
// Example logic: Alternate settings based on split index
return new LowCodeSaveOptions();
}
}
}
}
```
### See Also
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
