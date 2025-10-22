##Aspose::Cells::JsonSaveOptions class
'Aspose::Cells::JsonSaveOptions class. Represents the options of saving the workbook as a json file in C++.'
## JsonSaveOptions class
Represents the options of saving the workbook as a json file.
```cpp
class JsonSaveOptions : public Aspose::Cells::SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAlwaysExportAsJsonObject()](./getalwaysexportasjsonobject/) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportArea()](./getexportarea/) | Gets or sets the exporting range. |
| [GetExportAsString()](./getexportasstring/) | Exports the string value of the cells to json. |
| [GetExportEmptyCells()](./getexportemptycells/) | Indicates whether exporting empty cells as null. |
| [GetExportHyperlinkType()](./getexporthyperlinktype/) | Represents the type of exporting hyperlink to json. |
| [GetExportNestedStructure()](./getexportnestedstructure/) | Exported as parent-child hierarchy [Json](../../aspose.cells.json/) structure. |
| [GetExportStylePool()](./getexportstylepool/) | Indicates whether to export styles collectively or individually to each cell. |
| [GetHasHeaderRow()](./gethasheaderrow/) | Indicates whether the range contains header row. |
| [GetIndent()](./getindent/) | Indicates the indent. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSchemas()](./getschemas/) | The original json schema of each worksheet. |
| [GetSheetIndexes()](./getsheetindexes/) | Represents the indexes of exported sheets. |
| [GetSkipEmptyRows()](./getskipemptyrows/) | Indicates whether skipping emtpy rows. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetToExcelStruct()](./gettoexcelstruct/) | Indicates whether converting to json struct of the Excel file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [JsonSaveOptions()](./jsonsaveoptions/) | Creates options for saving json file. |
| [JsonSaveOptions(JsonSaveOptions_Impl* impl)](./jsonsaveoptions/) | Constructs from an implementation object. |
| [JsonSaveOptions(const JsonSaveOptions\& src)](./jsonsaveoptions/) | Copy constructor. |
| [JsonSaveOptions(const SaveOptions\& src)](./jsonsaveoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const JsonSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetAlwaysExportAsJsonObject(bool value)](./setalwaysexportasjsonobject/) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportArea(const CellArea\& value)](./setexportarea/) | Gets or sets the exporting range. |
| [SetExportAsString(bool value)](./setexportasstring/) | Exports the string value of the cells to json. |
| [SetExportEmptyCells(bool value)](./setexportemptycells/) | Indicates whether exporting empty cells as null. |
| [SetExportHyperlinkType(JsonExportHyperlinkType value)](./setexporthyperlinktype/) | Represents the type of exporting hyperlink to json. |
| [SetExportNestedStructure(bool value)](./setexportnestedstructure/) | Exported as parent-child hierarchy [Json](../../aspose.cells.json/) structure. |
| [SetExportStylePool(bool value)](./setexportstylepool/) | Indicates whether to export styles collectively or individually to each cell. |
| [SetHasHeaderRow(bool value)](./sethasheaderrow/) | Indicates whether the range contains header row. |
| [SetIndent(const U16String\& value)](./setindent/) | Indicates the indent. |
| [SetIndent(const char16_t* value)](./setindent/) | Indicates the indent. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSchemas(const Vector \<U16String\>\& value)](./setschemas/) | The original json schema of each worksheet. |
| [SetSheetIndexes(const Vector \<int32_t\>\& value)](./setsheetindexes/) | Represents the indexes of exported sheets. |
| [SetSkipEmptyRows(bool value)](./setskipemptyrows/) | Indicates whether skipping emtpy rows. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetToExcelStruct(bool value)](./settoexcelstruct/) | Indicates whether converting to json struct of the Excel file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~JsonSaveOptions()](./~jsonsaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
