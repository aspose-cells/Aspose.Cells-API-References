##Class XmlSaveOptions
Aspose.Cells.XmlSaveOptions class. Represents the options of saving the workbook as an xml file
## XmlSaveOptions class
Represents the options of saving the workbook as an xml file.
```csharp
public class XmlSaveOptions : SaveOptions
```
## Constructors
| Name | Description |
| --- | --- |
| [XmlSaveOptions](xmlsaveoptions/)() | Creates options for saving xml file. |
## Properties
| Name | Description |
| --- | --- |
| [CachedFileFolder](../../aspose.cells/saveoptions/cachedfilefolder/) { get; set; } | The folder for temporary files that may be used as data cache.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CheckExcelRestriction](../../aspose.cells/saveoptions/checkexcelrestriction/) { get; set; } | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ClearData](../../aspose.cells/saveoptions/cleardata/) { get; set; } | Make the workbook empty after saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [CreateDirectory](../../aspose.cells/saveoptions/createdirectory/) { get; set; } | If true and the directory does not exist, the directory will be automatically created before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [DataAsAttribute](../../aspose.cells/xmlsaveoptions/dataasattribute/) { get; set; } | Indicates whether exporting data as attributes of element. |
| [EncryptDocumentProperties](../../aspose.cells/saveoptions/encryptdocumentproperties/) { get; set; } | Indicates whether encrypt document properties when saving as .xls file. The default value is true.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ExportArea](../../aspose.cells/xmlsaveoptions/exportarea/) { get; set; } | Gets or sets the exporting range. |
| [HasHeaderRow](../../aspose.cells/xmlsaveoptions/hasheaderrow/) { get; set; } | Indicates whether the range contains header row. |
| [MergeAreas](../../aspose.cells/saveoptions/mergeareas/) { get; set; } | Indicates whether merge the areas of conditional formatting and validation before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [RefreshChartCache](../../aspose.cells/saveoptions/refreshchartcache/) { get; set; } | Indicates whether refreshing chart cache data(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SaveFormat](../../aspose.cells/saveoptions/saveformat/) { get; } | Gets the save file format.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SheetIndexes](../../aspose.cells/xmlsaveoptions/sheetindexes/) { get; set; } | Represents the indexes of exported sheets. |
| [SheetNameAsElementName](../../aspose.cells/xmlsaveoptions/sheetnameaselementname/) { get; set; } | Indicates whether exporting sheet's name as the name of the element. |
| [SortExternalNames](../../aspose.cells/saveoptions/sortexternalnames/) { get; set; } | Indicates whether sorting external defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [SortNames](../../aspose.cells/saveoptions/sortnames/) { get; set; } | Indicates whether sorting defined names before saving file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [UpdateSmartArt](../../aspose.cells/saveoptions/updatesmartart/) { get; set; } | Indicates whether updating smart art setting. The default value is false.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [ValidateMergedAreas](../../aspose.cells/saveoptions/validatemergedareas/) { get; set; } | Indicates whether validate merged cells before saving the file.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [WarningCallback](../../aspose.cells/saveoptions/warningcallback/) { get; set; } | Gets or sets warning callback.(Inherited from [`SaveOptions`](../saveoptions/).) |
| [XmlMapName](../../aspose.cells/xmlsaveoptions/xmlmapname/) { get; set; } | Indicates whether exporting xml map in the file. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class XmlSaveOptionsDemo
{
public static void XmlSaveOptionsExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Fill some data in the worksheet
worksheet.Cells["A1"].PutValue("Header1");
worksheet.Cells["B1"].PutValue("Header2");
worksheet.Cells["A2"].PutValue("Data1");
worksheet.Cells["B2"].PutValue("Data2");
// Create an instance of XmlSaveOptions
XmlSaveOptions saveOptions = new XmlSaveOptions();
// Setting properties
saveOptions.ExportArea = new CellArea { StartRow = 0, EndRow = 1, StartColumn = 0, EndColumn = 1 };
saveOptions.HasHeaderRow = true;
saveOptions.SheetIndexes = new int[] { 0 };
saveOptions.XmlMapName = "MyXmlMap";
saveOptions.SheetNameAsElementName = true;
saveOptions.DataAsAttribute = false;
saveOptions.ClearData = false;
saveOptions.CachedFileFolder = "C:\\Temp";
saveOptions.ValidateMergedAreas = true;
saveOptions.MergeAreas = false;
saveOptions.SortNames = true;
saveOptions.SortExternalNames = false;
saveOptions.RefreshChartCache = true;
saveOptions.UpdateSmartArt = false;
// Save the workbook as an XML file
workbook.Save("XmlSaveOptionsExample.xml", saveOptions);
return;
}
}
}
```
### See Also
* class [SaveOptions](../saveoptions/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
