##Class OdsSaveOptions
Aspose.Cells.OdsSaveOptions class. Represents the options of saving ods file
## OdsSaveOptions class
Represents the options of saving ods file.
```csharp
public class OdsSaveOptions : SaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [OdsSaveOptions](odssaveoptions/#constructor)() | Creates the options of saving ods file. |
| [OdsSaveOptions](odssaveoptions/#constructor_1)(SaveFormat) | Creates the options of saving ods file. |
## Properties
| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [GeneratorType](../../aspose.cells/odssaveoptions/generatortype/) { get; set; } | Gets and sets the generator of the ods file. |
| [IgnorePivotTables](../../aspose.cells/odssaveoptions/ignorepivottables/) { get; set; } | Indicates whether saving pivot tables. |
| [IsStrictSchema11](../../aspose.cells/odssaveoptions/isstrictschema11/) { get; set; } | (**Obsolete.**) Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [OdfStrictVersion](../../aspose.cells/odssaveoptions/odfstrictversion/) { get; set; } | Gets and sets the ODF version. |
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
using Aspose.Cells.Ods;
using System;
public class OdsSaveOptionsDemo
{
public static void OdsSaveOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Hello World");
// Create an instance of OdsSaveOptions
OdsSaveOptions saveOptions = new OdsSaveOptions();
// Setting properties
saveOptions.GeneratorType = OdsGeneratorType.LibreOffice;
saveOptions.IsStrictSchema11 = true;
saveOptions.OdfStrictVersion = OpenDocumentFormatVersionType.Odf12;
saveOptions.ClearData = false;
saveOptions.CachedFileFolder = @"C:\Temp";
saveOptions.ValidateMergedAreas = true;
saveOptions.MergeAreas = true;
saveOptions.SortNames = true;
saveOptions.SortExternalNames = true;
saveOptions.RefreshChartCache = true;
saveOptions.UpdateSmartArt = false;
// Save the workbook as ODS file with the specified options
workbook.Save("OdsSaveOptionsExample.ods", saveOptions);
return;
}
}
}
```
### See Also
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
