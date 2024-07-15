---
title: XmlSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of saving the workbook as an xml file.
type: docs
url: /nodejs-cpp/xmlsaveoptions/
---

## XmlSaveOptions class

Represents the options of saving the workbook as an xml file.

```javascript
class XmlSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving xml file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getSheetIndexes()](#getSheetIndexes--)| Represents the indexes of exported sheets. |
| [setSheetIndexes(number[])](#setSheetIndexes-numberarray-)| Represents the indexes of exported sheets. |
| [getExportArea()](#getExportArea--)| Gets or sets the exporting range. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| Gets or sets the exporting range. |
| [getHasHeaderRow()](#getHasHeaderRow--)| Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| Indicates whether the range contains header row. |
| [getXmlMapName()](#getXmlMapName--)| Indicates whether exporting xml map in the file. |
| [setXmlMapName(string)](#setXmlMapName-string-)| Indicates whether exporting xml map in the file. |
| [getSheetNameAsElementName()](#getSheetNameAsElementName--)| Indicates whether exporting sheet's name as the name of the element. |
| [setSheetNameAsElementName(boolean)](#setSheetNameAsElementName-boolean-)| Indicates whether exporting sheet's name as the name of the element. |
| [getDataAsAttribute()](#getDataAsAttribute--)| Indicates whether exporting data as attributes of element. |
| [setDataAsAttribute(boolean)](#setDataAsAttribute-boolean-)| Indicates whether exporting data as attributes of element. |
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


### constructor() {#constructor--}

Creates options for saving xml file.

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

### getXmlMapName() {#getXmlMapName--}

Indicates whether exporting xml map in the file.

```javascript
getXmlMapName() : string;
```


### setXmlMapName(string) {#setXmlMapName-string-}

Indicates whether exporting xml map in the file.

```javascript
setXmlMapName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getSheetNameAsElementName() {#getSheetNameAsElementName--}

Indicates whether exporting sheet's name as the name of the element.

```javascript
getSheetNameAsElementName() : boolean;
```


### setSheetNameAsElementName(boolean) {#setSheetNameAsElementName-boolean-}

Indicates whether exporting sheet's name as the name of the element.

```javascript
setSheetNameAsElementName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataAsAttribute() {#getDataAsAttribute--}

Indicates whether exporting data as attributes of element.

```javascript
getDataAsAttribute() : boolean;
```


### setDataAsAttribute(boolean) {#setDataAsAttribute-boolean-}

Indicates whether exporting data as attributes of element.

```javascript
setDataAsAttribute(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

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


