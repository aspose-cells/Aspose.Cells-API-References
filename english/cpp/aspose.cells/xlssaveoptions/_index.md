---
title: Aspose::Cells::XlsSaveOptions class
linktitle: XlsSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::XlsSaveOptions class. Represents the save options for the Excel 97-2003 file format: xls and xlt in C++.'
type: docs
weight: 17000
url: /cpp/aspose.cells/xlssaveoptions/
---
## XlsSaveOptions class


Represents the save options for the Excel 97-2003 file format: xls and xlt.

```cpp
class XlsSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [GetCheckExcelRestriction()](../saveoptions/getcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetLightCellsDataProvider()](./getlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [GetMatchColor()](./getmatchcolor/) | Indicates whether matching font color because there are 56 colors in the standard color palette. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [GetWpsCompatibility()](./getwpscompatibility/) |  **(Deprecated)** Indicates whether to make the xls more compatible with WPS. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const XlsSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The folder for temporary files that may be used as data cache. |
| [SetCheckExcelRestriction(bool value)](../saveoptions/setcheckexcelrestriction/) | Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetLightCellsDataProvider(LightCellsDataProvider* value)](./setlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [SetMatchColor(bool value)](./setmatchcolor/) | Indicates whether matching font color because there are 56 colors in the standard color palette. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [SetWpsCompatibility(bool value)](./setwpscompatibility/) |  **(Deprecated)** Indicates whether to make the xls more compatible with WPS. |
| [XlsSaveOptions()](./xlssaveoptions/) | Creates options for saving Excel 97-2003 xls file. |
| explicit [XlsSaveOptions(SaveFormat saveFormat)](./xlssaveoptions/) | Creates options for saving Excel 97-2003 xls/xlt file. |
| [XlsSaveOptions(XlsSaveOptions_Impl* impl)](./xlssaveoptions/) | Constructs from an implementation object. |
| [XlsSaveOptions(const XlsSaveOptions\& src)](./xlssaveoptions/) | Copy constructor. |
| [XlsSaveOptions(const SaveOptions\& src)](./xlssaveoptions/) | Constructs from a parent object. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
| [~XlsSaveOptions()](./~xlssaveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
