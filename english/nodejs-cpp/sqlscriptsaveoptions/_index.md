---
title: SqlScriptSaveOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of saving sql.
type: docs
url: /nodejs-cpp/sqlscriptsaveoptions/
---

## SqlScriptSaveOptions class

Represents the options of saving sql.

```javascript
class SqlScriptSaveOptions extends SaveOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates options for saving sql file. |
| [constructor(SaveOptions)](#constructor-saveoptions-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getCheckIfTableExists()](#getCheckIfTableExists--)| Check if the table name exists before creating |
| [setCheckIfTableExists(boolean)](#setCheckIfTableExists-boolean-)| Check if the table name exists before creating |
| [getColumnTypeMap()](#getColumnTypeMap--)| Gets and sets the map of column type for different database. |
| [setColumnTypeMap(SqlScriptColumnTypeMap)](#setColumnTypeMap-sqlscriptcolumntypemap-)| Gets and sets the map of column type for different database. |
| [getCheckAllDataForColumnType()](#getCheckAllDataForColumnType--)| Check all data to find columns' data type. |
| [setCheckAllDataForColumnType(boolean)](#setCheckAllDataForColumnType-boolean-)| Check all data to find columns' data type. |
| [getAddBlankLineBetweenRows()](#getAddBlankLineBetweenRows--)| Insert blank line between each data. |
| [setAddBlankLineBetweenRows(boolean)](#setAddBlankLineBetweenRows-boolean-)| Insert blank line between each data. |
| [getSeparator()](#getSeparator--)| Gets and sets character separator of sql script. |
| [setSeparator(string)](#setSeparator-string-)| Gets and sets character separator of sql script. |
| [getOperatorType()](#getOperatorType--)| Gets and sets the operator type of sql. |
| [setOperatorType(SqlScriptOperatorType)](#setOperatorType-sqlscriptoperatortype-)| Gets and sets the operator type of sql. |
| [getPrimaryKey()](#getPrimaryKey--)| Represents which column is primary key of the data table. |
| [setPrimaryKey(number)](#setPrimaryKey-number-)| Represents which column is primary key of the data table. |
| [getCreateTable()](#getCreateTable--)| Indicates whether exporting sql of creating table. |
| [setCreateTable(boolean)](#setCreateTable-boolean-)| Indicates whether exporting sql of creating table. |
| [getIdName()](#getIdName--)| Gets and sets the name of id column. |
| [setIdName(string)](#setIdName-string-)| Gets and sets the name of id column. |
| [getStartId()](#getStartId--)| Gets and sets the start id. |
| [setStartId(number)](#setStartId-number-)| Gets and sets the start id. |
| [getTableName()](#getTableName--)| Gets and sets the table name. |
| [setTableName(string)](#setTableName-string-)| Gets and sets the table name. |
| [getExportAsString()](#getExportAsString--)| Indicates whether exporting all data as string value. |
| [setExportAsString(boolean)](#setExportAsString-boolean-)| Indicates whether exporting all data as string value. |
| [getSheetIndexes()](#getSheetIndexes--)| Represents the indexes of exported sheets. |
| [setSheetIndexes(number[])](#setSheetIndexes-numberarray-)| Represents the indexes of exported sheets. |
| [getExportArea()](#getExportArea--)| Gets or sets the exporting range. |
| [setExportArea(CellArea)](#setExportArea-cellarea-)| Gets or sets the exporting range. |
| [getHasHeaderRow()](#getHasHeaderRow--)| Indicates whether the range contains header row. |
| [setHasHeaderRow(boolean)](#setHasHeaderRow-boolean-)| Indicates whether the range contains header row. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
| [getCheckExcelRestriction()](#getCheckExcelRestriction--)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [setCheckExcelRestriction(boolean)](#setCheckExcelRestriction-boolean-)| Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated. |
| [getUpdateSmartArt()](#getUpdateSmartArt--)| Indicates whether updating smart art setting. The default value is false. |
| [setUpdateSmartArt(boolean)](#setUpdateSmartArt-boolean-)| Indicates whether updating smart art setting. The default value is false. |
| [getEncryptDocumentProperties()](#getEncryptDocumentProperties--)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |
| [setEncryptDocumentProperties(boolean)](#setEncryptDocumentProperties-boolean-)| Indicates whether encrypt document properties when saving as .xls file. The default value is true. |


### constructor() {#constructor--}

Creates options for saving sql file.

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

### getCheckIfTableExists() {#getCheckIfTableExists--}

Check if the table name exists before creating

```javascript
getCheckIfTableExists() : boolean;
```


### setCheckIfTableExists(boolean) {#setCheckIfTableExists-boolean-}

Check if the table name exists before creating

```javascript
setCheckIfTableExists(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getColumnTypeMap() {#getColumnTypeMap--}

Gets and sets the map of column type for different database.

```javascript
getColumnTypeMap() : SqlScriptColumnTypeMap;
```


**Returns**

[SqlScriptColumnTypeMap](../sqlscriptcolumntypemap/)

### setColumnTypeMap(SqlScriptColumnTypeMap) {#setColumnTypeMap-sqlscriptcolumntypemap-}

Gets and sets the map of column type for different database.

```javascript
setColumnTypeMap(value: SqlScriptColumnTypeMap) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlScriptColumnTypeMap](../sqlscriptcolumntypemap/) | The value to set. |

### getCheckAllDataForColumnType() {#getCheckAllDataForColumnType--}

Check all data to find columns' data type.

```javascript
getCheckAllDataForColumnType() : boolean;
```


**Remarks**

The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

### setCheckAllDataForColumnType(boolean) {#setCheckAllDataForColumnType-boolean-}

Check all data to find columns' data type.

```javascript
setCheckAllDataForColumnType(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

The default value is false, we only check the first row for performance. If this property is true and the columns contains mixed value type, the columns' type will be text.

### getAddBlankLineBetweenRows() {#getAddBlankLineBetweenRows--}

Insert blank line between each data.

```javascript
getAddBlankLineBetweenRows() : boolean;
```


**Remarks**

If [Separator](../separator/) is '\n' , it's better to set this property as true to increase readability.

### setAddBlankLineBetweenRows(boolean) {#setAddBlankLineBetweenRows-boolean-}

Insert blank line between each data.

```javascript
setAddBlankLineBetweenRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

If [Separator](../separator/) is '\n' , it's better to set this property as true to increase readability.

### getSeparator() {#getSeparator--}

Gets and sets character separator of sql script.

```javascript
getSeparator() : string;
```


**Remarks**

Only can be ' ' or '\n'. If the

### setSeparator(string) {#setSeparator-string-}

Gets and sets character separator of sql script.

```javascript
setSeparator(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

Only can be ' ' or '\n'. If the

### getOperatorType() {#getOperatorType--}

Gets and sets the operator type of sql.

```javascript
getOperatorType() : SqlScriptOperatorType;
```


**Returns**

[SqlScriptOperatorType](../sqlscriptoperatortype/)

### setOperatorType(SqlScriptOperatorType) {#setOperatorType-sqlscriptoperatortype-}

Gets and sets the operator type of sql.

```javascript
setOperatorType(value: SqlScriptOperatorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SqlScriptOperatorType](../sqlscriptoperatortype/) | The value to set. |

### getPrimaryKey() {#getPrimaryKey--}

Represents which column is primary key of the data table.

```javascript
getPrimaryKey() : number;
```


### setPrimaryKey(number) {#setPrimaryKey-number-}

Represents which column is primary key of the data table.

```javascript
setPrimaryKey(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getCreateTable() {#getCreateTable--}

Indicates whether exporting sql of creating table.

```javascript
getCreateTable() : boolean;
```


### setCreateTable(boolean) {#setCreateTable-boolean-}

Indicates whether exporting sql of creating table.

```javascript
setCreateTable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getIdName() {#getIdName--}

Gets and sets the name of id column.

```javascript
getIdName() : string;
```


**Remarks**

If this property is set , a column will be inserted with automatical increment int value.

### setIdName(string) {#setIdName-string-}

Gets and sets the name of id column.

```javascript
setIdName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If this property is set , a column will be inserted with automatical increment int value.

### getStartId() {#getStartId--}

Gets and sets the start id.

```javascript
getStartId() : number;
```


**Remarks**

Only works when [IdName](../idname/) is set.

### setStartId(number) {#setStartId-number-}

Gets and sets the start id.

```javascript
setStartId(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only works when [IdName](../idname/) is set.

### getTableName() {#getTableName--}

Gets and sets the table name.

```javascript
getTableName() : string;
```


### setTableName(string) {#setTableName-string-}

Gets and sets the table name.

```javascript
setTableName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getExportAsString() {#getExportAsString--}

Indicates whether exporting all data as string value.

```javascript
getExportAsString() : boolean;
```


### setExportAsString(boolean) {#setExportAsString-boolean-}

Indicates whether exporting all data as string value.

```javascript
setExportAsString(value: boolean) : void;
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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


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

### getCheckExcelRestriction() {#getCheckExcelRestriction--}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
getCheckExcelRestriction() : boolean;
```


### setCheckExcelRestriction(boolean) {#setCheckExcelRestriction-boolean-}

Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K, it will be truncated.

```javascript
setCheckExcelRestriction(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

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


