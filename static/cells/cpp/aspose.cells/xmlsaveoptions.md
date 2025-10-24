##Aspose::Cells::XmlSaveOptions class
'Aspose::Cells::XmlSaveOptions class. Represents the options of saving the workbook as an xml file in C++.'
## XmlSaveOptions class
Represents the options of saving the workbook as an xml file.
```cpp
class XmlSaveOptions : public Aspose::Cells::SaveOptions
```
## Methods
| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetDataAsAttribute()](./getdataasattribute/) | Indicates whether exporting data as attributes of element. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportArea()](./getexportarea/) | Gets or sets the exporting range. |
| [GetHasHeaderRow()](./gethasheaderrow/) | Indicates whether the range contains header row. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSheetIndexes()](./getsheetindexes/) | Represents the indexes of exported sheets. |
| [GetSheetNameAsElementName()](./getsheetnameaselementname/) | Indicates whether exporting sheet's name as the name of the element. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [GetXmlMapName()](./getxmlmapname/) | Indicates whether exporting xml map in the file. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const XmlSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetDataAsAttribute(bool value)](./setdataasattribute/) | Indicates whether exporting data as attributes of element. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportArea(const CellArea\& value)](./setexportarea/) | Gets or sets the exporting range. |
| [SetHasHeaderRow(bool value)](./sethasheaderrow/) | Indicates whether the range contains header row. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSheetIndexes(const Vector \<int32_t\>\& value)](./setsheetindexes/) | Represents the indexes of exported sheets. |
| [SetSheetNameAsElementName(bool value)](./setsheetnameaselementname/) | Indicates whether exporting sheet's name as the name of the element. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SetXmlMapName(const U16String\& value)](./setxmlmapname/) | Indicates whether exporting xml map in the file. |
| [SetXmlMapName(const char16_t* value)](./setxmlmapname/) | Indicates whether exporting xml map in the file. |
| [XmlSaveOptions()](./xmlsaveoptions/) | Creates options for saving xml file. |
| [XmlSaveOptions(XmlSaveOptions_Impl* impl)](./xmlsaveoptions/) | Constructs from an implementation object. |
| [XmlSaveOptions(const XmlSaveOptions\& src)](./xmlsaveoptions/) | Copy constructor. |
| [XmlSaveOptions(const SaveOptions\& src)](./xmlsaveoptions/) | Constructs from a parent object. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
| [~XmlSaveOptions()](./~xmlsaveoptions/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
