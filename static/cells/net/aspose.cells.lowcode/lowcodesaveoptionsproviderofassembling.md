##Class LowCodeSaveOptionsProviderOfAssembling
Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfAssembling class. Implementation to provide save options which save split parts to files and the path of resultant file are named asit may contains directories PathHeaderSheetPrefixSheetIndexor SheetName SplitPartPrefixSplitPartIndexPathTail
## LowCodeSaveOptionsProviderOfAssembling class
Implementation to provide save options which save split parts to files and the path of resultant file are named as(it may contains directories): [`PathHeader`](./pathheader/)+[`SheetPrefix`](./sheetprefix/)+SheetIndex(or SheetName) +[`SplitPartPrefix`](./splitpartprefix/)+SplitPartIndex+[`PathTail`](./pathtail/).
```csharp
public class LowCodeSaveOptionsProviderOfAssembling : AbstractLowCodeSaveOptionsProvider
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfAssembling](lowcodesaveoptionsproviderofassembling/)() | The default constructor. |
## Properties
| Name | Description |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/) { get; set; } | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index(or name) and corresponding prefix will not be added to the file path. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsplitpartalways/) { get; set; } | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix will not be added to the file path. |
| [PathHeader](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathheader/) { get; set; } | Header part(before added content of sheet and split part) of file path. |
| [PathTail](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/pathtail/) { get; set; } | Tailing part(after sequence numbers) of file path. It should include extension of file name. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/saveoptionstemplate/) { get; set; } | The template for creating instance of save options in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/) { get; set; } | Offset of sheet's index between what used in file path and its actual value([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetprefix/) { get; set; } | Prefix for the index of worksheet. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/) { get; set; } | Offset of split part's index between what used in file path and its actual value([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/) { get; set; } | Prefix for the index of split part. |
| [UseSheetName](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/) { get; set; } | Whether builds the file path with sheet name instead of sheet index. Default value is false. |
## Methods
| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Releases resources after processing currently split part.(Inherited from [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/getsaveoptions/)(SplitPartInfo) | Gets the save options from which to get the output settings for currently split part. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Saving;
public class LowCodeClassLowCodeSaveOptionsProviderOfAssemblingDemo
{
public static void Run()
{
// Create a new workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
for (int i = 0; i < 100; i++)
{
worksheet.Cells[i, 0].Value = $"Data {i + 1}";
}
// Initialize and configure the save options provider
LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling
{
PathHeader = "SplitOutput/",
PathTail = "_Part.xlsx",
UseSheetName = true,
SheetPrefix = "SHEET-",
SplitPartPrefix = "PART-",
BuildPathWithSheetAlways = true,
BuildPathWithSplitPartAlways = true,
SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
};
// Configure XLSX save options with splitting using LowCodeSaveOptions
LowCodeSaveOptions saveOptions = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Xlsx
};
// Save workbook with provider-enabled options using correct save format
workbook.Save("LowCodeSaveOptionsProviderOfAssemblingDemo_Output.xlsx", saveOptions.SaveFormat);
}
}
}
```
### See Also
* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
