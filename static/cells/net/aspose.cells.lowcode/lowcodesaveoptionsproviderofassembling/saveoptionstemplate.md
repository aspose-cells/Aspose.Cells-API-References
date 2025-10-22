##LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate
LowCodeSaveOptionsProviderOfAssembling property. The template for creating instance of save options in GetSaveOptions
## LowCodeSaveOptionsProviderOfAssembling.SaveOptionsTemplate property
The template for creating instance of save options in [`GetSaveOptions`](../getsaveoptions/).
```csharp
public LowCodeSaveOptions SaveOptionsTemplate { get; set; }
```
### Remarks
If the template has been specified, then the created instance will copy all setting from it and update the output file accordingly.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Saving;
using System;
public class LowCodeSaveOptionsProviderOfAssemblingPropertySaveOptionsTemplateDemo
{
public static void Run()
{
// Create a new workbook with two worksheets
Workbook workbook = new Workbook();
workbook.Worksheets.Add("Sheet2");
Worksheet worksheet1 = workbook.Worksheets[0];
Worksheet worksheet2 = workbook.Worksheets[1];
worksheet1.Cells["A1"].PutValue("Sheet1 Content");
worksheet2.Cells["A1"].PutValue("Sheet2 Content");
// Create an instance of LowCodeSaveOptionsProviderOfAssembling
var provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "Output/Sheet",
PathTail = ".xlsx",
BuildPathWithSheetAlways = true,
UseSheetName = false
};
// Display initial SaveOptionsTemplate state
Console.WriteLine("Initial SaveOptionsTemplate is " + (provider.SaveOptionsTemplate == null ? "null" : "set"));
// Configure SaveOptionsTemplate with encryption
provider.SaveOptionsTemplate = new LowCodeSaveOptions();
Console.WriteLine("SaveOptionsTemplate configured");
// Create LowCode save options
var saveOptions = new LowCodeSaveOptions();
// Save workbook using configured provider (will generate separate files per sheet)
workbook.Save("output_combined.xlsx", saveOptions.SaveFormat);
Console.WriteLine("Demo executed successfully. Check output files.");
}
}
}
```
### See Also
* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)
