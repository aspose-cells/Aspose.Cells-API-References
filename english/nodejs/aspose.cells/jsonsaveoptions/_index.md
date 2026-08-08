---
title: "JsonSaveOptions"
linktitle: "JsonSaveOptions"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the options of saving the workbook as a json file."
type: docs
weight: 1960
url: /nodejs/aspose.cells/jsonsaveoptions/
---

## JsonSaveOptions class

Represents the options of saving the workbook as a json file.

```js
new JsonSaveOptions()
```

Creates options for saving json file.

## Methods

| Name | Description |
| --- | --- |
| [getAlwaysExportAsJsonObject()](#getalwaysexportasjsonobject) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [getCachedFileFolder()](#getcachedfilefolder) | The cached file folder is used to store some large data. |
| [getCheckExcelRestriction()](#getcheckexcelrestriction) |  |
| [getClearData()](#getcleardata) | Make the workbook empty after saving the file. |
| [getCreateDirectory()](#getcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [getEncryptDocumentProperties()](#getencryptdocumentproperties) |  |
| [getExportArea()](#getexportarea) | Gets or sets the exporting range. |
| [getExportAsString()](#getexportasstring) | Exports the string value of the cells to json. |
| [getExportEmptyCells()](#getexportemptycells) | Indicates whether exporting empty cells as null. |
| [getExportHyperlinkType()](#getexporthyperlinktype) | Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constan |
| [getExportNestedStructure()](#getexportnestedstructure) | Exported as parent-child hierarchy Json structure. |
| [getExportStylePool()](#getexportstylepool) |  |
| [getIndent()](#getindent) | Indicates the indent. If the indent is null or empty, the exported json is not formatted. |
| [getMergeAreas()](#getmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [getRefreshChartCache()](#getrefreshchartcache) | Indicates whether refreshing chart cache data |
| [getSaveFormat()](#getsaveformat) | Gets the save file format. The value of the property is SaveFormat integer constant. |
| [getSchemas()](#getschemas) |  |
| [getSheetIndexes()](#getsheetindexes) | Represents the indexes of exported sheets. |
| [getSkipEmptyRows()](#getskipemptyrows) | Indicates whether skipping emtpy rows. |
| [getSortExternalNames()](#getsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [getSortNames()](#getsortnames) | Indicates whether sorting defined names before saving file. |
| [getToExcelStruct()](#gettoexcelstruct) | Indicates whether converting to json struct of the Excel file. Only for converting range to JSON. |
| [getUpdateSmartArt()](#getupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [getValidateMergedAreas()](#getvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [getWarningCallback()](#getwarningcallback) | Gets or sets warning callback. |
| [hasHeaderRow()](#hasheaderrow) | Indicates whether the range contains header row. |
| [setAlwaysExportAsJsonObject()](#setalwaysexportasjsonobject) | Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [setCachedFileFolder()](#setcachedfilefolder) | The cached file folder is used to store some large data. |
| [setCheckExcelRestriction()](#setcheckexcelrestriction) |  |
| [setClearData()](#setcleardata) | Make the workbook empty after saving the file. |
| [setCreateDirectory()](#setcreatedirectory) | If true and the directory does not exist, the directory will be automatically created before saving the file. The defaul |
| [setEncryptDocumentProperties()](#setencryptdocumentproperties) |  |
| [setExportArea()](#setexportarea) | Gets or sets the exporting range. |
| [setExportAsString()](#setexportasstring) | Exports the string value of the cells to json. |
| [setExportEmptyCells()](#setexportemptycells) | Indicates whether exporting empty cells as null. |
| [setExportHyperlinkType()](#setexporthyperlinktype) | Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constan |
| [setExportNestedStructure()](#setexportnestedstructure) | Exported as parent-child hierarchy Json structure. |
| [setExportStylePool()](#setexportstylepool) |  |
| [setHasHeaderRow()](#sethasheaderrow) | Indicates whether the range contains header row. |
| [setIndent()](#setindent) | Indicates the indent. If the indent is null or empty, the exported json is not formatted. |
| [setMergeAreas()](#setmergeareas) | Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is  |
| [setRefreshChartCache()](#setrefreshchartcache) | Indicates whether refreshing chart cache data |
| [setSchemas()](#setschemas) |  |
| [setSheetIndexes()](#setsheetindexes) | Represents the indexes of exported sheets. |
| [setSkipEmptyRows()](#setskipemptyrows) | Indicates whether skipping emtpy rows. |
| [setSortExternalNames()](#setsortexternalnames) | Indicates whether sorting external defined names before saving file. |
| [setSortNames()](#setsortnames) | Indicates whether sorting defined names before saving file. |
| [setToExcelStruct()](#settoexcelstruct) | Indicates whether converting to json struct of the Excel file. Only for converting range to JSON. |
| [setUpdateSmartArt()](#setupdatesmartart) | Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSm |
| [setValidateMergedAreas()](#setvalidatemergedareas) | Indicates whether validate merged cells before saving the file. The default value is false. |
| [setWarningCallback()](#setwarningcallback) | Gets or sets warning callback. |

### getAlwaysExportAsJsonObject() {#getalwaysexportasjsonobject}

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

### getCachedFileFolder() {#getcachedfilefolder}

The cached file folder is used to store some large data.

### getCheckExcelRestriction() {#getcheckexcelrestriction}

### getClearData() {#getcleardata}

Make the workbook empty after saving the file.

### getCreateDirectory() {#getcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### getEncryptDocumentProperties() {#getencryptdocumentproperties}

### getExportArea() {#getexportarea}

Gets or sets the exporting range.

### getExportAsString() {#getexportasstring}

Exports the string value of the cells to json.

### getExportEmptyCells() {#getexportemptycells}

Indicates whether exporting empty cells as null.

### getExportHyperlinkType() {#getexporthyperlinktype}

Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constant. The default value is JsonExportHyperlinkType.DISPLAY_STRING;

### getExportNestedStructure() {#getexportnestedstructure}

Exported as parent-child hierarchy Json structure.

### getExportStylePool() {#getexportstylepool}

### getIndent() {#getindent}

Indicates the indent. If the indent is null or empty, the exported json is not formatted.

### getMergeAreas() {#getmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### getRefreshChartCache() {#getrefreshchartcache}

Indicates whether refreshing chart cache data

### getSaveFormat() {#getsaveformat}

Gets the save file format. The value of the property is SaveFormat integer constant.

### getSchemas() {#getschemas}

### getSheetIndexes() {#getsheetindexes}

Represents the indexes of exported sheets.

### getSkipEmptyRows() {#getskipemptyrows}

Indicates whether skipping emtpy rows.

### getSortExternalNames() {#getsortexternalnames}

Indicates whether sorting external defined names before saving file.

### getSortNames() {#getsortnames}

Indicates whether sorting defined names before saving file.

### getToExcelStruct() {#gettoexcelstruct}

Indicates whether converting to json struct of the Excel file. Only for converting range to JSON.

### getUpdateSmartArt() {#getupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getValidateMergedAreas() {#getvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### getWarningCallback() {#getwarningcallback}

Gets or sets warning callback.

### hasHeaderRow() {#hasheaderrow}

Indicates whether the range contains header row.

### setAlwaysExportAsJsonObject() {#setalwaysexportasjsonobject}

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

### setCachedFileFolder() {#setcachedfilefolder}

The cached file folder is used to store some large data.

### setCheckExcelRestriction() {#setcheckexcelrestriction}

### setClearData() {#setcleardata}

Make the workbook empty after saving the file.

### setCreateDirectory() {#setcreatedirectory}

If true and the directory does not exist, the directory will be automatically created before saving the file. The default value is false.

### setEncryptDocumentProperties() {#setencryptdocumentproperties}

### setExportArea() {#setexportarea}

Gets or sets the exporting range.

### setExportAsString() {#setexportasstring}

Exports the string value of the cells to json.

### setExportEmptyCells() {#setexportemptycells}

Indicates whether exporting empty cells as null.

### setExportHyperlinkType() {#setexporthyperlinktype}

Represents the type of exporting hyperlink to json. The value of the property is JsonExportHyperlinkType integer constant. The default value is JsonExportHyperlinkType.DISPLAY_STRING;

### setExportNestedStructure() {#setexportnestedstructure}

Exported as parent-child hierarchy Json structure.

### setExportStylePool() {#setexportstylepool}

### setHasHeaderRow() {#sethasheaderrow}

Indicates whether the range contains header row.

### setIndent() {#setindent}

Indicates the indent. If the indent is null or empty, the exported json is not formatted.

### setMergeAreas() {#setmergeareas}

Indicates whether merge the areas of conditional formatting and validation before saving the file. The default value is false.

### setRefreshChartCache() {#setrefreshchartcache}

Indicates whether refreshing chart cache data

### setSchemas() {#setschemas}

### setSheetIndexes() {#setsheetindexes}

Represents the indexes of exported sheets.

### setSkipEmptyRows() {#setskipemptyrows}

Indicates whether skipping emtpy rows.

### setSortExternalNames() {#setsortexternalnames}

Indicates whether sorting external defined names before saving file.

### setSortNames() {#setsortnames}

Indicates whether sorting defined names before saving file.

### setToExcelStruct() {#settoexcelstruct}

Indicates whether converting to json struct of the Excel file. Only for converting range to JSON.

### setUpdateSmartArt() {#setupdatesmartart}

Indicates whether updating smart art setting. The default value is false. Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setValidateMergedAreas() {#setvalidatemergedareas}

Indicates whether validate merged cells before saving the file. The default value is false.

### setWarningCallback() {#setwarningcallback}

Gets or sets warning callback.
