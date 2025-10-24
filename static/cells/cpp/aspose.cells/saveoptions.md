##Aspose::Cells::SaveOptions class
'Aspose::Cells::SaveOptions class. Represents all save options in C++.'
## SaveOptions class
Represents all save options.
```cpp
class SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](./getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](./getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](./getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](./getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEncryptDocumentProperties()](./getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetMergeAreas()](./getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](./getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](./getsaveformat/) | Gets the save file format. |
| [GetSortExternalNames()](./getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](./getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](./getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](./getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](./getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const SaveOptions\& src)](./operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](./saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](./saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](./setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](./setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](./setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](./setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEncryptDocumentProperties(bool value)](./setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetMergeAreas(bool value)](./setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](./setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSortExternalNames(bool value)](./setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](./setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](./setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](./setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](./setwarningcallback/) | Gets or sets warning callback. |
| [~SaveOptions()](./~saveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
