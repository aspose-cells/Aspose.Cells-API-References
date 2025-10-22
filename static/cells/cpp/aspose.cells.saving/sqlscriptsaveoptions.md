##Aspose::Cells::Saving::SqlScriptSaveOptions class
'Aspose::Cells::Saving::SqlScriptSaveOptions class. Represents the options of saving sql in C++.'
## SqlScriptSaveOptions class
Represents the options of saving sql.
```cpp
class SqlScriptSaveOptions : public Aspose::Cells::SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetAddBlankLineBetweenRows()](./getaddblanklinebetweenrows/) | Insert blank line between each data. |
| [GetCachedFileFolder()](../../aspose.cells/saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckAllDataForColumnType()](./getcheckalldataforcolumntype/) | Check all data to find columns' data type. |
| [GetCheckExcelRestriction()](../../aspose.cells/saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetCheckIfTableExists()](./getcheckiftableexists/) | Check if the table name exists before creating. |
| [GetClearData()](../../aspose.cells/saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetColumnTypeMap()](./getcolumntypemap/) | Gets and sets the map of column type for different database. |
| [GetCreateDirectory()](../../aspose.cells/saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetCreateTable()](./getcreatetable/) | Indicates whether exporting sql of creating table. |
| [GetEncryptDocumentProperties()](../../aspose.cells/saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportArea()](./getexportarea/) | Gets or sets the exporting range. |
| [GetExportAsString()](./getexportasstring/) | Indicates whether exporting all data as string value. |
| [GetHasHeaderRow()](./gethasheaderrow/) | Indicates whether the range contains header row. |
| [GetIdName()](./getidname/) | Gets and sets the name of id column. |
| [GetMergeAreas()](../../aspose.cells/saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetOperatorType()](./getoperatortype/) | Gets and sets the operator type of sql. |
| [GetPrimaryKey()](./getprimarykey/) | Represents which column is primary key of the data table. |
| [GetRefreshChartCache()](../../aspose.cells/saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../../aspose.cells/saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSeparator()](./getseparator/) | Gets and sets character separator of sql script. |
| [GetSheetIndexes()](./getsheetindexes/) | Represents the indexes of exported sheets. |
| [GetSortExternalNames()](../../aspose.cells/saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../../aspose.cells/saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetStartId()](./getstartid/) | Gets and sets the start id. |
| [GetTableName()](./gettablename/) | Gets and sets the table name. |
| [GetUpdateSmartArt()](../../aspose.cells/saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../../aspose.cells/saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../../aspose.cells/saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SqlScriptSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../../aspose.cells/saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../../aspose.cells/saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../../aspose.cells/saveoptions/saveoptions/) | Copy constructor. |
| [SetAddBlankLineBetweenRows(bool value)](./setaddblanklinebetweenrows/) | Insert blank line between each data. |
| [SetCachedFileFolder(const U16String\& value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../../aspose.cells/saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckAllDataForColumnType(bool value)](./setcheckalldataforcolumntype/) | Check all data to find columns' data type. |
| [SetCheckExcelRestriction(bool value)](../../aspose.cells/saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetCheckIfTableExists(bool value)](./setcheckiftableexists/) | Check if the table name exists before creating. |
| [SetClearData(bool value)](../../aspose.cells/saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetColumnTypeMap(const SqlScriptColumnTypeMap\& value)](./setcolumntypemap/) | Gets and sets the map of column type for different database. |
| [SetCreateDirectory(bool value)](../../aspose.cells/saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetCreateTable(bool value)](./setcreatetable/) | Indicates whether exporting sql of creating table. |
| [SetEncryptDocumentProperties(bool value)](../../aspose.cells/saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportArea(const CellArea\& value)](./setexportarea/) | Gets or sets the exporting range. |
| [SetExportAsString(bool value)](./setexportasstring/) | Indicates whether exporting all data as string value. |
| [SetHasHeaderRow(bool value)](./sethasheaderrow/) | Indicates whether the range contains header row. |
| [SetIdName(const U16String\& value)](./setidname/) | Gets and sets the name of id column. |
| [SetIdName(const char16_t* value)](./setidname/) | Gets and sets the name of id column. |
| [SetMergeAreas(bool value)](../../aspose.cells/saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetOperatorType(SqlScriptOperatorType value)](./setoperatortype/) | Gets and sets the operator type of sql. |
| [SetPrimaryKey(int32_t value)](./setprimarykey/) | Represents which column is primary key of the data table. |
| [SetRefreshChartCache(bool value)](../../aspose.cells/saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSeparator(char16_t value)](./setseparator/) | Gets and sets character separator of sql script. |
| [SetSheetIndexes(const Vector \<int32_t\>\& value)](./setsheetindexes/) | Represents the indexes of exported sheets. |
| [SetSortExternalNames(bool value)](../../aspose.cells/saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../../aspose.cells/saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetStartId(int32_t value)](./setstartid/) | Gets and sets the start id. |
| [SetTableName(const U16String\& value)](./settablename/) | Gets and sets the table name. |
| [SetTableName(const char16_t* value)](./settablename/) | Gets and sets the table name. |
| [SetUpdateSmartArt(bool value)](../../aspose.cells/saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../../aspose.cells/saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../../aspose.cells/saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SqlScriptSaveOptions()](./sqlscriptsaveoptions/) | Creates options for saving sql file. |
| [SqlScriptSaveOptions(SqlScriptSaveOptions_Impl* impl)](./sqlscriptsaveoptions/) | Constructs from an implementation object. |
| [SqlScriptSaveOptions(const SqlScriptSaveOptions\& src)](./sqlscriptsaveoptions/) | Copy constructor. |
| [SqlScriptSaveOptions(const SaveOptions\& src)](./sqlscriptsaveoptions/) | Constructs from a parent object. |
| [~SaveOptions()](../../aspose.cells/saveoptions/~saveoptions/) | Destructor. |
| [~SqlScriptSaveOptions()](./~sqlscriptsaveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [SaveOptions](../../aspose.cells/saveoptions/)
* Namespace [Aspose::Cells::Saving](../)
* Library [Aspose.Cells for C++](../../)
