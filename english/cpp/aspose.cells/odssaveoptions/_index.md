﻿---
title: Aspose::Cells::OdsSaveOptions class
linktitle: OdsSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::OdsSaveOptions class. Represents the options of saving ods file in C++.'
type: docs
weight: 10500
url: /cpp/aspose.cells/odssaveoptions/
---
## OdsSaveOptions class


Represents the options of saving ods file.

```cpp
class OdsSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The cached file folder is used to store some large data. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetGeneratorType()](./getgeneratortype/) | Gets and sets the generator of the ods file. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetOdfStrictVersion()](./getodfstrictversion/) | Gets and sets the ODF version. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsStrictSchema11()](./isstrictschema11/) |  **(Deprecated)** Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [OdsSaveOptions()](./odssaveoptions/) | Creates the options of saving ods file. |
| explicit [OdsSaveOptions(SaveFormat saveFormat)](./odssaveoptions/) | Creates the options of saving ods file. |
| [OdsSaveOptions(OdsSaveOptions_Impl* impl)](./odssaveoptions/) | Constructs from an implementation object. |
| [OdsSaveOptions(const OdsSaveOptions\& src)](./odssaveoptions/) | Copy constructor. |
| [OdsSaveOptions(const SaveOptions\& src)](./odssaveoptions/) | Constructs from a parent object. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const OdsSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetGeneratorType(OdsGeneratorType value)](./setgeneratortype/) | Gets and sets the generator of the ods file. |
| [SetIsStrictSchema11(bool value)](./setisstrictschema11/) |  **(Deprecated)** Indicates whether the ods file should be saved as ODF format version 1.1. Default is false. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetOdfStrictVersion(OpenDocumentFormatVersionType value)](./setodfstrictversion/) | Gets and sets the ODF version. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~OdsSaveOptions()](./~odssaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
