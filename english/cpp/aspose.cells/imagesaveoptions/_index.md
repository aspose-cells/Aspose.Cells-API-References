---
title: Aspose::Cells::ImageSaveOptions class
linktitle: ImageSaveOptions
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::ImageSaveOptions class. Represents image save options. For advanced usage, please use WorkbookRender or SheetRender in C++.'
type: docs
weight: 8400
url: /cpp/aspose.cells/imagesaveoptions/
---
## ImageSaveOptions class


Represents image save options. For advanced usage, please use WorkbookRender or SheetRender.

```cpp
class ImageSaveOptions : public Aspose::Cells::SaveOptions
```

## Methods

| Method | Description |
| --- | --- |
| [GetCachedFileFolder()](../saveoptions/getcachedfilefolder/) | The cached file folder is used to store some large data. |
| [GetClearData()](../saveoptions/getcleardata/) | Make the workbook empty after saving the file. |
| [GetCreateDirectory()](../saveoptions/getcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [GetImageOrPrintOptions()](./getimageorprintoptions/) | Additional image creation options. |
| [GetMergeAreas()](../saveoptions/getmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [GetRefreshChartCache()](../saveoptions/getrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [GetSaveFormat()](../saveoptions/getsaveformat/) | Gets the save file format. |
| [GetSortExternalNames()](../saveoptions/getsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [GetSortNames()](../saveoptions/getsortnames/) | Indicates whether sorting defined names before saving file. |
| [GetUpdateSmartArt()](../saveoptions/getupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [GetValidateMergedAreas()](../saveoptions/getvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [GetWarningCallback()](../saveoptions/getwarningcallback/) | Gets or sets warning callback. |
| [ImageSaveOptions()](./imagesaveoptions/) | Creates the options for saving image file. |
| explicit [ImageSaveOptions(SaveFormat saveFormat)](./imagesaveoptions/) | Creates the options for saving image file. |
| [ImageSaveOptions(ImageSaveOptions_Impl* impl)](./imagesaveoptions/) | Constructs from an implementation object. |
| [ImageSaveOptions(const ImageSaveOptions\& src)](./imagesaveoptions/) | Copy constructor. |
| [ImageSaveOptions(const SaveOptions\& src)](./imagesaveoptions/) | Constructs from a parent object. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const ImageSaveOptions\& src)](./operator_asm/) | operator= |
| [operator=(const SaveOptions\& src)](../saveoptions/operator_asm/) | operator= |
| [SaveOptions(SaveOptions_Impl* impl)](../saveoptions/saveoptions/) | Constructs from an implementation object. |
| [SaveOptions(const SaveOptions\& src)](../saveoptions/saveoptions/) | Copy constructor. |
| [SetCachedFileFolder(const U16String\& value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetCachedFileFolder(const char16_t* value)](../saveoptions/setcachedfilefolder/) | The cached file folder is used to store some large data. |
| [SetClearData(bool value)](../saveoptions/setcleardata/) | Make the workbook empty after saving the file. |
| [SetCreateDirectory(bool value)](../saveoptions/setcreatedirectory/) | If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [SetMergeAreas(bool value)](../saveoptions/setmergeareas/) | Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [SetRefreshChartCache(bool value)](../saveoptions/setrefreshchartcache/) | Indicates whether refreshing chart cache data. |
| [SetSortExternalNames(bool value)](../saveoptions/setsortexternalnames/) | Indicates whether sorting external defined names before saving file. |
| [SetSortNames(bool value)](../saveoptions/setsortnames/) | Indicates whether sorting defined names before saving file. |
| [SetUpdateSmartArt(bool value)](../saveoptions/setupdatesmartart/) | Indicates whether updating smart art setting. The default value is false. |
| [SetValidateMergedAreas(bool value)](../saveoptions/setvalidatemergedareas/) | Indicates whether validate merged cells before saving the file. |
| [SetWarningCallback(IWarningCallback* value)](../saveoptions/setwarningcallback/) | Gets or sets warning callback. |
| [~ImageSaveOptions()](./~imagesaveoptions/) | Destructor. |
| [~SaveOptions()](../saveoptions/~saveoptions/) | Destructor. |
## Fields

| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also

* Class [SaveOptions](../saveoptions/)
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
