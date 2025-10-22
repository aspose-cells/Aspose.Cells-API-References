##Class TxtSaveOptions
Aspose.Cells.TxtSaveOptions class. Represents the save options for csv/tab delimited/other text format
## TxtSaveOptions class
Represents the save options for csv/tab delimited/other text format.
```csharp
public class TxtSaveOptions : SaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [TxtSaveOptions](txtsaveoptions/#constructor)() | Creates text file save options. |
| [TxtSaveOptions](txtsaveoptions/#constructor_1)(SaveFormat) | Creates text file save options. |
## Properties
| Name | Description |
| --- | --- |
| [AlwaysQuoted](../../aspose.cells/txtsaveoptions/alwaysquoted/) { get; set; } | (**Obsolete.**) Indicates whether always adding '"' for each field. If true then all values will be quoted; If false then values will only be quoted when needed(for example, when values contain special characters such as '"' , '\n' or separator character). Default is false. |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Encoding](../../aspose.cells/txtsaveoptions/encoding/) { get; set; } | Gets and sets the default encoding. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExportAllSheets](../../aspose.cells/txtsaveoptions/exportallsheets/) { get; set; } | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
| [ExportArea](../../aspose.cells/txtsaveoptions/exportarea/) { get; set; } | The range of cells to be exported. |
| [ExportQuotePrefix](../../aspose.cells/txtsaveoptions/exportquoteprefix/) { get; set; } | Indicates whether the single quote sign should be exported as part of the value of one cell when [`QuotePrefix`](../style/quoteprefix/) is true for it. Default is false. |
| [FormatStrategy](../../aspose.cells/txtsaveoptions/formatstrategy/) { get; set; } | Gets and sets the format strategy when exporting the cell value as string. |
| [KeepSeparatorsForBlankRow](../../aspose.cells/txtsaveoptions/keepseparatorsforblankrow/) { get; set; } | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [LightCellsDataProvider](../../aspose.cells/txtsaveoptions/lightcellsdataprovider/) { get; set; } | The data provider for saving workbook in light mode. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [QuoteType](../../aspose.cells/txtsaveoptions/quotetype/) { get; set; } | Gets or sets how to quote values in the exported text file. |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [Separator](../../aspose.cells/txtsaveoptions/separator/) { get; set; } | Gets and sets char Delimiter of text file. |
| [SeparatorString](../../aspose.cells/txtsaveoptions/separatorstring/) { get; set; } | Gets and sets a string value as separator. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [TrimLeadingBlankRowAndColumn](../../aspose.cells/txtsaveoptions/trimleadingblankrowandcolumn/) { get; set; } | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [TrimTailingBlankCells](../../aspose.cells/txtsaveoptions/trimtailingblankcells/) { get; set; } | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
using System.Text;
public class TxtSaveOptionsDemo
{
public static void TxtSaveOptionsExample()
{
// Create a workbook with some data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Name");
worksheet.Cells["B1"].PutValue("Age");
worksheet.Cells["A2"].PutValue("John Doe");
worksheet.Cells["B2"].PutValue(30);
worksheet.Cells["A3"].PutValue("Jane Smith");
worksheet.Cells["B3"].PutValue(25);
// Create TxtSaveOptions object and set properties
TxtSaveOptions saveOptions = new TxtSaveOptions
{
Separator = ',',
SeparatorString = ",",
Encoding = Encoding.UTF8,
AlwaysQuoted = false,
QuoteType = TxtValueQuoteType.Normal,
FormatStrategy = CellValueFormatStrategy.DisplayStyle,
TrimLeadingBlankRowAndColumn = true,
TrimTailingBlankCells = false,
KeepSeparatorsForBlankRow = false,
ExportArea = new CellArea { StartRow = 0, EndRow = 2, StartColumn = 0, EndColumn = 1 },
ExportQuotePrefix = false,
ExportAllSheets = false,
ClearData = false,
CachedFileFolder = "cache",
ValidateMergedAreas = true,
MergeAreas = true,
SortNames = true,
SortExternalNames = true,
RefreshChartCache = true,
UpdateSmartArt = false
};
// Save the workbook as a text file with the specified options
workbook.Save("TxtSaveOptionsExample.txt", saveOptions);
Console.WriteLine("Workbook saved successfully with TxtSaveOptions.");
}
}
}
```
### See Also
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
