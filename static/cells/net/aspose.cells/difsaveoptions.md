##Class DifSaveOptions
Aspose.Cells.DifSaveOptions class. Represents the options of saving dif file
## DifSaveOptions class
Represents the options of saving dif file.
```csharp
public class DifSaveOptions : SaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [DifSaveOptions](difsaveoptions/)() | Creates the options for saving DIF file. |
## Properties
| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class DifSaveOptionsDemo
{
public static void DifSaveOptionsExample()
{
// Create a new Workbook object
Workbook workbook = new Workbook();
// Add some data to the worksheet for demonstration purposes
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].PutValue("Sample Data");
// Create an instance of DifSaveOptions
DifSaveOptions saveOptions = new DifSaveOptions
{
// Set properties as per the JSON specification
ClearData = true,
CachedFileFolder = @"C:\Temp\CachedFiles",
ValidateMergedAreas = true,
MergeAreas = false,
CreateDirectory = true,
SortNames = true,
SortExternalNames = false,
RefreshChartCache = true,
UpdateSmartArt = false
};
// Save the workbook with the DifSaveOptions
workbook.Save("E:\\VSCellsForm\\DifSaveOptionsExample.dif", saveOptions);
// Output to console to indicate the process is complete
Console.WriteLine("Workbook saved successfully with DifSaveOptions.");
}
}
}
```
### See Also
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
