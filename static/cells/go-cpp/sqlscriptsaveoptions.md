##SqlScriptSaveOptions Class
'SqlScriptSaveOptions class. Encapsulates the object that represents sqlscriptsaveoptions in Go.'
## SqlScriptSaveOptions class
Represents the options of saving sql.
```go
type SqlScriptSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewSqlScriptSaveOptions](./newsqlscriptsaveoptions/) | Creates options for saving sql file. |
|[NewSqlScriptSaveOptions_SaveOptions](./newsqlscriptsaveoptions_saveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetCheckIfTableExists](./getcheckiftableexists/) | Check if the table name exists before creating |
|[SetCheckIfTableExists](./setcheckiftableexists/) | Check if the table name exists before creating |
|[GetColumnTypeMap](./getcolumntypemap/) | Gets and sets the map of column type for different database. |
|[SetColumnTypeMap](./setcolumntypemap/) | Gets and sets the map of column type for different database. |
|[GetCheckAllDataForColumnType](./getcheckalldataforcolumntype/) | Check all data to find columns' data type. |
|[SetCheckAllDataForColumnType](./setcheckalldataforcolumntype/) | Check all data to find columns' data type. |
|[GetAddBlankLineBetweenRows](./getaddblanklinebetweenrows/) | Insert blank line between each data. |
|[SetAddBlankLineBetweenRows](./setaddblanklinebetweenrows/) | Insert blank line between each data. |
|[GetSeparator](./getseparator/) | Gets and sets character separator of sql script. |
|[SetSeparator](./setseparator/) | Gets and sets character separator of sql script. |
|[GetOperatorType](./getoperatortype/) | Gets and sets the operator type of sql. |
|[SetOperatorType](./setoperatortype/) | Gets and sets the operator type of sql. |
|[GetPrimaryKey](./getprimarykey/) | Represents which column is primary key of the data table. |
|[SetPrimaryKey](./setprimarykey/) | Represents which column is primary key of the data table. |
|[GetCreateTable](./getcreatetable/) | Indicates whether exporting sql of creating table. |
|[SetCreateTable](./setcreatetable/) | Indicates whether exporting sql of creating table. |
|[GetIdName](./getidname/) | Gets and sets the name of id column. |
|[SetIdName](./setidname/) | Gets and sets the name of id column. |
|[GetStartId](./getstartid/) | Gets and sets the start id. |
|[SetStartId](./setstartid/) | Gets and sets the start id. |
|[GetTableName](./gettablename/) | Gets and sets the table name. |
|[SetTableName](./settablename/) | Gets and sets the table name. |
|[GetExportAsString](./getexportasstring/) | Indicates whether exporting all data as string value. |
|[SetExportAsString](./setexportasstring/) | Indicates whether exporting all data as string value. |
|[GetSheetIndexes](./getsheetindexes/) | Represents the indexes of exported sheets. |
|[SetSheetIndexes](./setsheetindexes/) | Represents the indexes of exported sheets. |
|[GetExportArea](./getexportarea/) | Gets or sets the exporting range. |
|[SetExportArea](./setexportarea/) | Gets or sets the exporting range. |
|[GetHasHeaderRow](./gethasheaderrow/) | Indicates whether the range contains header row. |
|[SetHasHeaderRow](./sethasheaderrow/) | Indicates whether the range contains header row. |
|[GetSaveFormat](./getsaveformat/) | Gets the save file format. |
|[GetClearData](./getcleardata/) | Make the workbook empty after saving the file. |
|[SetClearData](./setcleardata/) | Make the workbook empty after saving the file. |
|[GetCachedFileFolder](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[SetCachedFileFolder](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
|[GetValidateMergedAreas](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[SetValidateMergedAreas](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
|[GetMergeAreas](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[SetMergeAreas](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
|[GetCreateDirectory](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[SetCreateDirectory](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
|[GetSortNames](./getsortnames/) | Indicates whether sorting defined names before saving file. |
|[SetSortNames](./setsortnames/) | Indicates whether sorting defined names before saving file. |
|[GetSortExternalNames](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[SetSortExternalNames](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
|[GetRefreshChartCache](./getrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[SetRefreshChartCache](./setrefreshchartcache/) | Indicates whether refreshing chart cache data |
|[GetCheckExcelRestriction](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[SetCheckExcelRestriction](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects.For example, excel does not allow inputting string value longer than 32K.When you input a value longer than 32K, it will be truncated. |
|[GetUpdateSmartArt](./getupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[SetUpdateSmartArt](./setupdatesmartart/) | Indicates whether updating smart art setting.The default value is false. |
|[GetEncryptDocumentProperties](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
|[SetEncryptDocumentProperties](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file.The default value is true. |
