---
title: "OoxmlSaveOptions"
linktitle: "OoxmlSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options of saving office open xml file."
type: docs
weight: 2460
url: /nodejs/aspose.cells/ooxmlsaveoptions/
---

## OoxmlSaveOptions class

Represents the options of saving office open xml file.

```js
new OoxmlSaveOptions()
```

Creates the options for saving office open xml file.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(saveFormat)](#constructor-overload1) | Creates the options for saving office open xml file. |
| [getAsFlatOpc()](#getasflatopc) |  |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCompressionType()](#getcompressiontype) | Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant.Th |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getEmbedOoxmlAsOleObject()](#getembedooxmlasoleobject) | Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject. |
| [getEnableZip64()](#getenablezip64) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExportCellName()](#getexportcellname) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL S |
| [getLightCellsDataProvider()](#getlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getUpdateZoom()](#getupdatezoom) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesT |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWpsCompatibility()](#getwpscompatibility) |  |
| [setAsFlatOpc()](#setasflatopc) |  |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCompressionType()](#setcompressiontype) | Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant.Th |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setEmbedOoxmlAsOleObject()](#setembedooxmlasoleobject) | Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject. |
| [setEnableZip64()](#setenablezip64) | Always use ZIP64 extensions when writing zip archives, even when unnecessary. |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExportCellName()](#setexportcellname) | Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL S |
| [setLightCellsDataProvider()](#setlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setUpdateZoom()](#setupdatezoom) | Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesT |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWpsCompatibility()](#setwpscompatibility) |  |

### constructor_overload$1(saveFormat) {#constructor-overload1}

Creates the options for saving office open xml file.

| Parameter | Type | Description |
| --- | --- | --- |
| saveFormat | Number | SaveFormat |

### getAsFlatOpc() {#getasflatopc}

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCompressionType() {#getcompressiontype}

Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant.The default value is OoxmlCompressionType.Level2.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getEmbedOoxmlAsOleObject() {#getembedooxmlasoleobject}

Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject.

### getEnableZip64() {#getenablezip64}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExportCellName() {#getexportcellname}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

### getLightCellsDataProvider() {#getlightcellsdataprovider}

The data provider for saving workbook in light mode.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getUpdateZoom() {#getupdatezoom}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. The default value is false for performance.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWpsCompatibility() {#getwpscompatibility}

### setAsFlatOpc() {#setasflatopc}

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCompressionType() {#setcompressiontype}

Gets and sets the compression type for ooxml file. The value of the property is OoxmlCompressionType integer constant.The default value is OoxmlCompressionType.Level2.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setEmbedOoxmlAsOleObject() {#setembedooxmlasoleobject}

Indicates whether embedding Ooxml files of OleObject as ole object. Only for OleObject.

### setEnableZip64() {#setenablezip64}

Always use ZIP64 extensions when writing zip archives, even when unnecessary.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExportCellName() {#setexportcellname}

Indicates if export cell name to Excel2007 .xlsx (.xlsm, .xltx, .xltm) file. If the output file may be accessed by SQL Server DTS, this value must be true. Setting the value to false will highly increase the performance and reduce the file size when creating large file. Default value is true.

### setLightCellsDataProvider() {#setlightcellsdataprovider}

The data provider for saving workbook in light mode.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateZoom() {#setupdatezoom}

Indicates whether update scaling factor before saving the file if the PageSetup.FitToPagesWide and PageSetup.FitToPagesTall properties control how the worksheet is scaled. The default value is false for performance.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWpsCompatibility() {#setwpscompatibility}
