﻿---
title: Aspose::Cells::OoxmlSaveOptions class
linktitle: OoxmlSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::OoxmlSaveOptions class. Represents the options of saving office open xml file in C++.'
type: docs
weight: 10800
url: /cpp/aspose.cells/ooxmlsaveoptions/
---
## OoxmlSaveOptions class


Represents the options of saving office open xml file.

```cpp
class OoxmlSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The cached file folder is used to store some large data. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCompressionType()](./getcompressiontype/) | Gets and sets the compression type for ooxml file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetEmbedOoxmlAsOleObject()](./getembedooxmlasoleobject/) | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [GetEnableZip64()](./getenablezip64/) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [GetEncryptDocumentProperties()](../saveoptions/getencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [GetExportCellName()](./getexportcellname/) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [GetLightCellsDataProvider()](./getlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetUpdateZoom()](./getupdatezoom/) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [OoxmlSaveOptions()](./ooxmlsaveoptions/) | Creates the options for saving office open xml file. |
| explicit [OoxmlSaveOptions(SaveFormat saveFormat)](./ooxmlsaveoptions/) | Creates the options for saving office open xml file. |
| [OoxmlSaveOptions(OoxmlSaveOptions_Impl* impl)](./ooxmlsaveoptions/) | Constructs from an implementation object. |
| [OoxmlSaveOptions(const OoxmlSaveOptions\& src)](./ooxmlsaveoptions/) | Copy constructor. |
| [OoxmlSaveOptions(const SaveOptions\& src)](./ooxmlsaveoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const OoxmlSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCompressionType(OoxmlCompressionType value)](./setcompressiontype/) | Gets and sets the compression type for ooxml file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetEmbedOoxmlAsOleObject(bool value)](./setembedooxmlasoleobject/) | Indicates whether embedding Ooxml files of OleObject as ole object. |
| [SetEnableZip64(bool value)](./setenablezip64/) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [SetEncryptDocumentProperties(bool value)](../saveoptions/setencryptdocumentproperties/) | Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [SetExportCellName(bool value)](./setexportcellname/) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true. |
| [SetLightCellsDataProvider(LightCellsDataProvider* value)](./setlightcellsdataprovider/) | The data provider for saving workbook in light mode. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetUpdateZoom(bool value)](./setupdatezoom/) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~OoxmlSaveOptions()](./~ooxmlsaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
