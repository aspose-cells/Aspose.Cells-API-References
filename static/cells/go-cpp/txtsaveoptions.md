##TxtSaveOptions Class
'TxtSaveOptions class. Encapsulates the object that represents txtsaveoptions in Go.'
## TxtSaveOptions class
Represents the save options for csv/tab delimited/other text format.
```go
type TxtSaveOptions struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
|[NewTxtSaveOptions](./newtxtsaveoptions/) | Creates text file save options. |
|[NewTxtSaveOptions_SaveFormat](./newtxtsaveoptions_saveformat/) | Creates text file save options. |
|[NewTxtSaveOptions_SaveOptions](./newtxtsaveoptions_saveoptions/) | Constructs from a parent object. |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetSeparator](./getseparator/) | Gets and sets char Delimiter of text file. |
|[SetSeparator](./setseparator/) | Gets and sets char Delimiter of text file. |
|[GetSeparatorString](./getseparatorstring/) | Gets and sets a string value as separator. |
|[SetSeparatorString](./setseparatorstring/) | Gets and sets a string value as separator. |
|[GetEncoding](./getencoding/) | Gets and sets the default encoding. |
|[SetEncoding](./setencoding/) | Gets and sets the default encoding. |
|[GetQuoteType](./getquotetype/) | Gets or sets how to quote values in the exported text file. |
|[SetQuoteType](./setquotetype/) | Gets or sets how to quote values in the exported text file. |
|[GetFormatStrategy](./getformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
|[SetFormatStrategy](./setformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
|[GetTrimLeadingBlankRowAndColumn](./gettrimleadingblankrowandcolumn/) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does.Default is true. |
|[SetTrimLeadingBlankRowAndColumn](./settrimleadingblankrowandcolumn/) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does.Default is true. |
|[GetTrimTailingBlankCells](./gettrimtailingblankcells/) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
|[SetTrimTailingBlankCells](./settrimtailingblankcells/) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
|[GetKeepSeparatorsForBlankRow](./getkeepseparatorsforblankrow/) | Indicates whether separators should be output for blank row.Default value is false so by default the content for blank row will be empty. |
|[SetKeepSeparatorsForBlankRow](./setkeepseparatorsforblankrow/) | Indicates whether separators should be output for blank row.Default value is false so by default the content for blank row will be empty. |
|[GetExportArea](./getexportarea/) | The range of cells to be exported. |
|[SetExportArea](./setexportarea/) | The range of cells to be exported. |
|[GetExportQuotePrefix](./getexportquoteprefix/) | Indicates whether the single quote sign should be exported as part of the value of one cellwhen Style.QuotePrefix is true for it. Default is false. |
|[SetExportQuotePrefix](./setexportquoteprefix/) | Indicates whether the single quote sign should be exported as part of the value of one cellwhen Style.QuotePrefix is true for it. Default is false. |
|[GetExportAllSheets](./getexportallsheets/) | Indicates whether exporting all sheets to the text file.If it is false, only export the activesheet, just like MS Excel. |
|[SetExportAllSheets](./setexportallsheets/) | Indicates whether exporting all sheets to the text file.If it is false, only export the activesheet, just like MS Excel. |
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
