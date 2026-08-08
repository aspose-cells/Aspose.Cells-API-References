---
title: "XlsSaveOptions"
linktitle: "XlsSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the save options for the Excel 97-2003 file format: xls and xlt."
type: docs
weight: 4760
url: /nodejs/aspose.cells/xlssaveoptions/
---

## XlsSaveOptions class

Represents the save options for the Excel 97-2003 file format: xls and xlt.

```js
new XlsSaveOptions()
```

Creates options for saving Excel 97-2003 xls file.

## Methods

| Name | Description |
| --- | --- |
| [constructor_overload$1(saveFormat)](#constructor-overload1) | Creates options for saving Excel 97-2003 xls/xlt file. |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getLightCellsDataProvider()](#getlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [getMatchColor()](#getmatchcolor) | Indicates whether matching font color because there are 56 colors in the standard color palette. |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWpsCompatibility()](#getwpscompatibility) |  |
| [isTemplate()](#istemplate) | Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with  |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setLightCellsDataProvider()](#setlightcellsdataprovider) | The data provider for saving workbook in light mode. |
| [setMatchColor()](#setmatchcolor) | Indicates whether matching font color because there are 56 colors in the standard color palette. |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setTemplate()](#settemplate) | Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with  |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWpsCompatibility()](#setwpscompatibility) |  |

### constructor_overload$1(saveFormat) {#constructor-overload1}

Creates options for saving Excel 97-2003 xls/xlt file.

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

### getLightCellsDataProvider() {#getlightcellsdataprovider}

The data provider for saving workbook in light mode.

### getMatchColor() {#getmatchcolor}

Indicates whether matching font color because there are 56 colors in the standard color palette.

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

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWpsCompatibility() {#getwpscompatibility}

### isTemplate() {#istemplate}

Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with corresponding save format(xlt for true and xls for false). This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setLightCellsDataProvider() {#setlightcellsdataprovider}

The data provider for saving workbook in light mode.

### setMatchColor() {#setmatchcolor}

Indicates whether matching font color because there are 56 colors in the standard color palette.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setTemplate() {#settemplate}

Indicates whether saving a template file. NOTE: This member is now obsolete. Instead, please create XlsSaveOptions with corresponding save format(xlt for true and xls for false). This method will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWpsCompatibility() {#setwpscompatibility}
