##Aspose::Cells::TxtSaveOptions class
'Aspose::Cells::TxtSaveOptions class. Represents the save options for csv/tab delimited/other text format in C++.'
## TxtSaveOptions class
Represents the save options for csv/tab delimited/other text format.
```cpp
class TxtSaveOptions : public Aspose::Cells::SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEncoding()](./getencoding/) | Gets and sets the default encoding. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportAllSheets()](./getexportallsheets/) | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
| [GetExportArea()](./getexportarea/) | The range of cells to be exported. |
| [GetExportQuotePrefix()](./getexportquoteprefix/) | Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is true for it. Default is false. |
| [GetFormatStrategy()](./getformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
| [GetKeepSeparatorsForBlankRow()](./getkeepseparatorsforblankrow/) | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [GetLightCellsDataProvider()](./getlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetQuoteType()](./getquotetype/) | Gets or sets how to quote values in the exported text file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSeparator()](./getseparator/) | Gets and sets char Delimiter of text file. |
| [GetSeparatorString()](./getseparatorstring/) | Gets and sets a string value as separator. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetTrimLeadingBlankRowAndColumn()](./gettrimleadingblankrowandcolumn/) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [GetTrimTailingBlankCells()](./gettrimtailingblankcells/) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const TxtSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEncoding(EncodingType value)](./setencoding/) | Gets and sets the default encoding. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportAllSheets(bool value)](./setexportallsheets/) | Indicates whether exporting all sheets to the text file. If it is false, only export the activesheet, just like MS Excel. |
| [SetExportArea(const CellArea\& value)](./setexportarea/) | The range of cells to be exported. |
| [SetExportQuotePrefix(bool value)](./setexportquoteprefix/) | Indicates whether the single quote sign should be exported as part of the value of one cell when Style.QuotePrefix is true for it. Default is false. |
| [SetFormatStrategy(CellValueFormatStrategy value)](./setformatstrategy/) | Gets and sets the format strategy when exporting the cell value as string. |
| [SetKeepSeparatorsForBlankRow(bool value)](./setkeepseparatorsforblankrow/) | Indicates whether separators should be output for blank row. Default value is false so by default the content for blank row will be empty. |
| [SetLightCellsDataProvider(LightCellsDataProvider* value)](./setlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetQuoteType(TxtValueQuoteType value)](./setquotetype/) | Gets or sets how to quote values in the exported text file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSeparator(char16_t value)](./setseparator/) | Gets and sets char Delimiter of text file. |
| [SetSeparatorString(const U16String\& value)](./setseparatorstring/) | Gets and sets a string value as separator. |
| [SetSeparatorString(const char16_t* value)](./setseparatorstring/) | Gets and sets a string value as separator. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetTrimLeadingBlankRowAndColumn(bool value)](./settrimleadingblankrowandcolumn/) | Indicates whether leading blank rows and columns should be trimmed like what ms excel does. Default is true. |
| [SetTrimTailingBlankCells(bool value)](./settrimtailingblankcells/) | Indicates whether tailing blank cells in one row should be trimmed. Default is false. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [TxtSaveOptions()](./txtsaveoptions/) | Creates text file save options. |
| explicit [TxtSaveOptions(SaveFormat saveFormat)](./txtsaveoptions/) | Creates text file save options. |
| [TxtSaveOptions(TxtSaveOptions_Impl* impl)](./txtsaveoptions/) | Constructs from an implementation object. |
| [TxtSaveOptions(const TxtSaveOptions\& src)](./txtsaveoptions/) | Copy constructor. |
| [TxtSaveOptions(const SaveOptions\& src)](./txtsaveoptions/) | Constructs from a parent object. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
| [~TxtSaveOptions()](./~txtsaveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
