---
title: "SvgSaveOptions"
linktitle: "SvgSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents Svg save options."
type: docs
weight: 3990
url: /nodejs/aspose.cells/svgsaveoptions/
---

## SvgSaveOptions class

Represents Svg save options. For advanced usage, please use WorkbookRender or SheetRender. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

```js
new SvgSaveOptions()
```

Creates the options for saving svg file. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(saveFormat)](#constructor-overload1) | Creates the options for saving svg file. NOTE: This constructor is now obsolete. Instead, please use SvgSaveOptions() co |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getImageOrPrintOptions()](#getimageorprintoptions) | Additional image creation options. For advanced usage, please use WorkbookRender or SheetRender. |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSheetIndex()](#getsheetindex) | Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This  |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getStreamProvider()](#getstreamprovider) | Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more  |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSheetIndex()](#setsheetindex) | Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This  |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setStreamProvider()](#setstreamprovider) | Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more  |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |

### constructor_overload$1(saveFormat) {#constructor-overload1}

Creates the options for saving svg file. NOTE: This constructor is now obsolete. Instead, please use SvgSaveOptions() constructor. This property will be removed 12 months later since August 2022. Aspose apologizes for any inconvenience you may have experienced.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | SaveFormat |

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getImageOrPrintOptions() {#getimageorprintoptions}

Additional image creation options. For advanced usage, please use WorkbookRender or SheetRender.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSheetIndex() {#getsheetindex}

Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getStreamProvider() {#getstreamprovider}

Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use WorkbookRender or SheetRender.

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSheetIndex() {#setsheetindex}

Gets and sets which worksheet should be exported. If the value is -1, the active worksheet will be exported. NOTE: This class is now obsolete. Instead, please use ImageSaveOptions class. This property will be removed 12 months later since March 2023. Aspose apologizes for any inconvenience you may have experienced.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setStreamProvider() {#setstreamprovider}

Gets or sets the IStreamProvider for exporting objects. If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use WorkbookRender or SheetRender.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.
