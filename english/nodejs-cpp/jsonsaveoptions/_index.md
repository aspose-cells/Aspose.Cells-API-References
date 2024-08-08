---
title: JsonSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of saving the workbook as a json file.
type: docs
url: /nodejs-cpp/jsonsaveoptions/
---

## JsonSaveOptions class

Represents the options of saving the workbook as a json file.

```javascript
class JsonSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving json file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getExportHyperlinkType()](#getExportHyperlinkType--)| Represents the type of exporting hyperlink to json. |
| [setExportHyperlinkType(JsonExportHyperlinkType)](#setExportHyperlinkType-jsonexporthyperlinktype-)| Represents the type of exporting hyperlink to json. |
| [getSkipEmptyRows()](#getSkipEmptyRows--)| Indicates whether skipping emtpy rows. |
| [setSkipEmptyRows(boolean)](#setSkipEmptyRows-boolean-)| Indicates whether skipping emtpy rows. |
| [getSheetIndexes()](#getSheetIndexes--)| Represents the indexes of exported sheets. |
| [setSheetIndexes(number[])](#setSheetIndexes-numberarray-)| Represents the indexes of exported sheets. |
| [getSchemas()](#getSchemas--)| The original json schema of each worksheet. |
| [setSchemas(string[])](#setSchemas-stringarray-)| The original json schema of each worksheet. |
| [getExportArea()](#getExportArea--)| Gets or sets the exporting range. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| Gets or sets the exporting range. |
| [getHasHeaderRow()](#getHasHeaderRow--)| Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| Indicates whether the range contains header row. |
| [getExportAsString()](#getExportAsString--)| Exports the string value of the cells to json. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| Exports the string value of the cells to json. |
| [getIndent()](#getIndent--)| Indicates the indent. |
| [setIndent(string)](#setIndent-string-)| Indicates the indent. |
| [getExportNestedStructure()](#getExportNestedStructure--)| Exported as parent-child hierarchy Json structure. |
| [setExportNestedStructure(boolean)](#setExportNestedStructure-boolean-)| Exported as parent-child hierarchy Json structure. |
| [getExportEmptyCells()](#getExportEmptyCells--)| Indicates whether exporting empty cells as null. |
| [setExportEmptyCells(boolean)](#setExportEmptyCells-boolean-)| Indicates whether exporting empty cells as null. |
| [getAlwaysExportAsJsonObject()](#getAlwaysExportAsJsonObject--)| Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [setAlwaysExportAsJsonObject(boolean)](#setAlwaysExportAsJsonObject-boolean-)| Indicates whether always exporting excel to json as object, even there is only a worksheet in the file. |
| [getToExcelStruct()](#getToExcelStruct--)| Indicates whether converting to json struct of the Excel file. |
| [setToExcelStruct(boolean)](#setToExcelStruct-boolean-)| Indicates whether converting to json struct of the Excel file. |
| [getSaveFormat()](#getSaveFormat--)| Gets the save file format. |
| [getClearData()](#getClearData--)| Make the workbook empty after saving the file. |
| [setClearData(boolean)](#setClearData-boolean-)| Make the workbook empty after saving the file. |
| [getCachedFileFolder()](#getCachedFileFolder--)| The cached file folder is used to store some large data. |
| [setCachedFileFolder(string)](#setCachedFileFolder-string-)| The cached file folder is used to store some large data. |
| [getValidateMergedAreas()](#getValidateMergedAreas--)| Indicates whether validate merged cells before saving the file. |
| [setValidateMergedAreas(boolean)](#setValidateMergedAreas-boolean-)| Indicates whether validate merged cells before saving the file. |
| [getMergeAreas()](#getMergeAreas--)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [setMergeAreas(boolean)](#setMergeAreas-boolean-)| Indicates whether merge the areas of conditional formatting and validation before saving the file. |
| [getCreateDirectory()](#getCreateDirectory--)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [setCreateDirectory(boolean)](#setCreateDirectory-boolean-)| If true and the directory does not exist, the directory will be automatically created before saving the file. |
| [getSortNames()](#getSortNames--)| Indicates whether sorting defined names before saving file. |
| [setSortNames(boolean)](#setSortNames-boolean-)| Indicates whether sorting defined names before saving file. |
| [getSortExternalNames()](#getSortExternalNames--)| Indicates whether sorting external defined names before saving file. |
| [setSortExternalNames(boolean)](#setSortExternalNames-boolean-)| Indicates whether sorting external defined names before saving file. |
| [getRefreshChartCache()](#getRefreshChartCache--)| Indicates whether refreshing chart cache data |
| [setRefreshChartCache(boolean)](#setRefreshChartCache-boolean-)| Indicates whether refreshing chart cache data |
| [setWarningCallback(IWarningCallback)](#setWarningCallback-iwarningcallback-)| Gets or sets warning callback. |
| [getWarningCallback()](#getWarningCallback--)| Gets or sets warning callback. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |


### constructor() {#constructor--}

Creates options for saving json file.

```javascript
constructor();
```


### constructor(SaveOptions) {#constructor-saveoptions-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: SaveOptions);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | SaveOptions | The parent object. |

### getExportHyperlinkType() {#getExportHyperlinkType--}

Represents the type of exporting hyperlink to json.

```javascript
getExportHyperlinkType() : JsonExportHyperlinkType;
```


**Returns**

[JsonExportHyperlinkType](../jsonexporthyperlinktype/)

**Remarks**

The default value is [JsonExportHyperlinkType.DisplayString](../jsonexporthyperlinktype.displaystring/);

### setExportHyperlinkType(JsonExportHyperlinkType) {#setExportHyperlinkType-jsonexporthyperlinktype-}

Represents the type of exporting hyperlink to json.

```javascript
setExportHyperlinkType(value: JsonExportHyperlinkType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [JsonExportHyperlinkType](../jsonexporthyperlinktype/) | The value to set. |

**Remarks**

The default value is [JsonExportHyperlinkType.DisplayString](../jsonexporthyperlinktype.displaystring/);

### getSkipEmptyRows() {#getSkipEmptyRows--}

Indicates whether skipping emtpy rows.

```javascript
getSkipEmptyRows() : boolean;
```


### setSkipEmptyRows(boolean) {#setSkipEmptyRows-boolean-}

Indicates whether skipping emtpy rows.

```javascript
setSkipEmptyRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSheetIndexes() {#getSheetIndexes--}

Represents the indexes of exported sheets.

```javascript
getSheetIndexes() : number[];
```


**Returns**

number[]

### setSheetIndexes(number[]) {#setSheetIndexes-numberarray-}

Represents the indexes of exported sheets.

```javascript
setSheetIndexes(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getSchemas() {#getSchemas--}

The original json schema of each worksheet.

```javascript
getSchemas() : string[];
```


**Returns**

string[]

### setSchemas(string[]) {#setSchemas-stringarray-}

The original json schema of each worksheet.

```javascript
setSchemas(value: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |

### getExportArea() {#getExportArea--}

Gets or sets the exporting range.

```javascript
getExportArea() : CellArea;
```


**Returns**

[CellArea](../cellarea/)

### setExportArea(CellArea) {#setExportArea-cellarea-}

Gets or sets the exporting range.

```javascript
setExportArea(value: CellArea) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellArea](../cellarea/) | The value to set. |

### getHasHeaderRow() {#getHasHeaderRow--}

Indicates whether the range contains header row.

```javascript
getHasHeaderRow() : boolean;
```


### setHasHeaderRow(boolean) {#setHasHeaderRow-boolean-}

Indicates whether the range contains header row.

```javascript
setHasHeaderRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportAsString() {#getExportAsString--}

Exports the string value of the cells to json.

```javascript
getExportAsString() : boolean;
```


### setExportAsString(boolean) {#setExportAsString-boolean-}

Exports the string value of the cells to json.

```javascript
setExportAsString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIndent() {#getIndent--}

Indicates the indent.

```javascript
getIndent() : string;
```


**Remarks**

If the indent is null or empty, the exported json is not formatted.

### setIndent(string) {#setIndent-string-}

Indicates the indent.

```javascript
setIndent(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If the indent is null or empty, the exported json is not formatted.

### getExportNestedStructure() {#getExportNestedStructure--}

Exported as parent-child hierarchy Json structure.

```javascript
getExportNestedStructure() : boolean;
```


### setExportNestedStructure(boolean) {#setExportNestedStructure-boolean-}

Exported as parent-child hierarchy Json structure.

```javascript
setExportNestedStructure(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportEmptyCells() {#getExportEmptyCells--}

Indicates whether exporting empty cells as null.

```javascript
getExportEmptyCells() : boolean;
```


### setExportEmptyCells(boolean) {#setExportEmptyCells-boolean-}

Indicates whether exporting empty cells as null.

```javascript
setExportEmptyCells(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAlwaysExportAsJsonObject() {#getAlwaysExportAsJsonObject--}

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

```javascript
getAlwaysExportAsJsonObject() : boolean;
```


### setAlwaysExportAsJsonObject(boolean) {#setAlwaysExportAsJsonObject-boolean-}

Indicates whether always exporting excel to json as object, even there is only a worksheet in the file.

```javascript
setAlwaysExportAsJsonObject(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getToExcelStruct() {#getToExcelStruct--}

Indicates whether converting to json struct of the Excel file.

```javascript
getToExcelStruct() : boolean;
```


**Remarks**

Only for converting range to JSON.

### setToExcelStruct(boolean) {#setToExcelStruct-boolean-}

Indicates whether converting to json struct of the Excel file.

```javascript
setToExcelStruct(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for converting range to JSON.

### getSaveFormat() {#getSaveFormat--}

Gets the save file format.

```javascript
getSaveFormat() : SaveFormat;
```


**Returns**

[SaveFormat](../saveformat/)

### getClearData() {#getClearData--}

Make the workbook empty after saving the file.

```javascript
getClearData() : boolean;
```


### setClearData(boolean) {#setClearData-boolean-}

Make the workbook empty after saving the file.

```javascript
setClearData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCachedFileFolder() {#getCachedFileFolder--}

The cached file folder is used to store some large data.

```javascript
getCachedFileFolder() : string;
```


### setCachedFileFolder(string) {#setCachedFileFolder-string-}

The cached file folder is used to store some large data.

```javascript
setCachedFileFolder(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getValidateMergedAreas() {#getValidateMergedAreas--}

Indicates whether validate merged cells before saving the file.

```javascript
getValidateMergedAreas() : boolean;
```


**Remarks**

The default value is false.

### setValidateMergedAreas(boolean) {#setValidateMergedAreas-boolean-}

Indicates whether validate merged cells before saving the file.

```javascript
setValidateMergedAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getMergeAreas() {#getMergeAreas--}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
getMergeAreas() : boolean;
```


**Remarks**

The default value is false.

### setMergeAreas(boolean) {#setMergeAreas-boolean-}

Indicates whether merge the areas of conditional formatting and validation before saving the file.

```javascript
setMergeAreas(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getCreateDirectory() {#getCreateDirectory--}

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
getCreateDirectory() : boolean;
```


**Remarks**

The default value is false.

### setCreateDirectory(boolean) {#setCreateDirectory-boolean-}

If true and the directory does not exist, the directory will be automatically created before saving the file.

```javascript
setCreateDirectory(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false.

### getSortNames() {#getSortNames--}

Indicates whether sorting defined names before saving file.

```javascript
getSortNames() : boolean;
```


### setSortNames(boolean) {#setSortNames-boolean-}

Indicates whether sorting defined names before saving file.

```javascript
setSortNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortExternalNames() {#getSortExternalNames--}

Indicates whether sorting external defined names before saving file.

```javascript
getSortExternalNames() : boolean;
```


### setSortExternalNames(boolean) {#setSortExternalNames-boolean-}

Indicates whether sorting external defined names before saving file.

```javascript
setSortExternalNames(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getRefreshChartCache() {#getRefreshChartCache--}

Indicates whether refreshing chart cache data

```javascript
getRefreshChartCache() : boolean;
```


### setRefreshChartCache(boolean) {#setRefreshChartCache-boolean-}

Indicates whether refreshing chart cache data

```javascript
setRefreshChartCache(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### setWarningCallback(IWarningCallback) {#setWarningCallback-iwarningcallback-}

Gets or sets warning callback.

```javascript
setWarningCallback(value: IWarningCallback) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [IWarningCallback](../iwarningcallback/) | The value to set. |

### getWarningCallback() {#getWarningCallback--}

Gets or sets warning callback.

```javascript
getWarningCallback() : IWarningCallback;
```


**Returns**

[IWarningCallback](../iwarningcallback/)

### getUpdateSmartArt() {#getUpdateSmartArt--}

Indicates whether updating smart art setting. The default value is false.

```javascript
getUpdateSmartArt() : boolean;
```


**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### setUpdateSmartArt(boolean) {#setUpdateSmartArt-boolean-}

Indicates whether updating smart art setting. The default value is false.

```javascript
setUpdateSmartArt(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only effects after calling Shape.GetResultOfSmartArt() method and the cached shapes exist in the template file.

### getEncryptDocumentProperties() {#getEncryptDocumentProperties--}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
getEncryptDocumentProperties() : boolean;
```


**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.

### setEncryptDocumentProperties(boolean) {#setEncryptDocumentProperties-boolean-}

Indicates whether encrypt document properties when saving as .xls file. The default value is true.

```javascript
setEncryptDocumentProperties(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for .xls,xlsx,xlsb and xlsm file.


