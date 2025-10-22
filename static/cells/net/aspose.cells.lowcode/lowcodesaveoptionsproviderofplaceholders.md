##Class LowCodeSaveOptionsProviderOfPlaceHolders
Aspose.Cells.LowCode.LowCodeSaveOptionsProviderOfPlaceHolders class. Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders
## LowCodeSaveOptionsProviderOfPlaceHolders class
Implementation to provide save options which save split parts to files and the path of resultant file are defined with placeholders.
```csharp
public class LowCodeSaveOptionsProviderOfPlaceHolders : AbstractLowCodeSaveOptionsProvider
```
## Constructors
| Name | Description |
| --- | --- |
| [LowCodeSaveOptionsProviderOfPlaceHolders](lowcodesaveoptionsproviderofplaceholders/)(string) | Instantiates an instance to provide save options according to specified templates. |
## Properties
| Name | Description |
| --- | --- |
| [BuildPathWithSheetAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/) { get; set; } | Whether add sheet index or name to file path always. Default value is false, that is, when there is only one sheet, the sheet index and name and corresponding prefix([`SheetNamePrefix`](./sheetnameprefix/)) will not be added to the file path. |
| [BuildPathWithSplitPartAlways](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/) { get; set; } | Whether add split part index to file path always. Default value is false, that is, when there is only one split part, the split part index and corresponding prefix([`SplitPartPrefix`](./splitpartprefix/)) will not be added to the file path. |
| [SaveOptionsTemplate](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/saveoptionstemplate/) { get; set; } | The template for creating instance of save options in [`GetSaveOptions`](./getsaveoptions/). |
| [SheetIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/) { get; set; } | Offset of sheet's index between what used in file path and its actual value([`SheetIndex`](../splitpartinfo/sheetindex/)). |
| [SheetIndexPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/) { get; set; } | Prefix for the index of worksheet. |
| [SheetNamePrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/) { get; set; } | Prefix for the index of worksheet. |
| [SplitPartIndexOffset](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/) { get; set; } | Offset of split part's index between what used in file path and its actual value([`PartIndex`](../splitpartinfo/partindex/)). |
| [SplitPartPrefix](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/) { get; set; } | Prefix for the index of split part. |
## Methods
| Name | Description |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodesaveoptionsprovider/finish/)(LowCodeSaveOptions) | Releases resources after processing currently split part.(Inherited from [`AbstractLowCodeSaveOptionsProvider`](../abstractlowcodesaveoptionsprovider/).) |
| override [GetSaveOptions](../../aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/getsaveoptions/)(SplitPartInfo) | Gets the save options from which to get the output settings for currently split part. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.LowCode;
using Aspose.Cells.Rendering;
public class LowCodeClassLowCodeSaveOptionsProviderOfPlaceHoldersDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Populate worksheet with sample data
for (int i = 0; i < 250; i++)
{
worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
}
// Create provider with path template containing placeholders
var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_Sheet_{sheet}_Part_{split}.xlsx");
// Configure provider properties
provider.SheetIndexOffset = 1;
provider.SplitPartIndexOffset = 1;
provider.SheetIndexPrefix = "S";
provider.SplitPartPrefix = "P";
provider.BuildPathWithSheetAlways = true;
provider.BuildPathWithSplitPartAlways = true;
// Configure save options template
provider.SaveOptionsTemplate = new LowCodeSaveOptions
{
SaveFormat = SaveFormat.Xlsx
};
// Configure image or print options for split rendering
var imgOrPrintOptions = new ImageOrPrintOptions
{
SaveFormat = SaveFormat.Pdf,
OnePagePerSheet = false,
PageIndex = 0,
PageCount = 1
};
// Create sheet render with split configuration
var sheetRender = new SheetRender(worksheet, imgOrPrintOptions);
sheetRender.ToImage(0, "output"); // This would normally split and save using provider
}
}
}
```
### See Also
* class [AbstractLowCodeSaveOptionsProvider](../abstractlowcodesaveoptionsprovider/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)
