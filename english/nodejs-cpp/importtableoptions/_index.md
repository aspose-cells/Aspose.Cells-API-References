---
title: ImportTableOptions
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the options of importing data into cells.
type: docs
url: /nodejs-cpp/importtableoptions/
---

## ImportTableOptions class

Represents the options of importing data into cells.

```javascript
class ImportTableOptions;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the default importing options. |

## Methods

| Method | Description |
| --- | --- |
| [getConvertGridStyle()](#getConvertGridStyle--)| Indicates whether apply the style of the grid view to cells. |
| [setConvertGridStyle(boolean)](#setConvertGridStyle-boolean-)| Indicates whether apply the style of the grid view to cells. |
| [getConvertNumericData()](#getConvertNumericData--)| Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [setConvertNumericData(boolean)](#setConvertNumericData-boolean-)| Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [getInsertRows()](#getInsertRows--)| Indicates whether new rows should be added for importing data records. |
| [setInsertRows(boolean)](#setInsertRows-boolean-)| Indicates whether new rows should be added for importing data records. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--)| Indicates whether shifting the first row down when inserting rows. |
| [setShiftFirstRowDown(boolean)](#setShiftFirstRowDown-boolean-)| Indicates whether shifting the first row down when inserting rows. |
| [isFieldNameShown()](#isFieldNameShown--)| Indicates whether field name should be imported. |
| [setIsFieldNameShown(boolean)](#setIsFieldNameShown-boolean-)| Indicates whether field name should be imported. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--)| Indicates whether exporting caption as field name |
| [setExportCaptionAsFieldName(boolean)](#setExportCaptionAsFieldName-boolean-)| Indicates whether exporting caption as field name |
| [getDateFormat()](#getDateFormat--)| Gets or sets date format string for cells with imported datetime values. |
| [setDateFormat(string)](#setDateFormat-string-)| Gets or sets date format string for cells with imported datetime values. |
| [getNumberFormats()](#getNumberFormats--)| Gets or sets the number formats |
| [setNumberFormats(string[])](#setNumberFormats-stringarray-)| Gets or sets the number formats |
| [getIsFormulas()](#getIsFormulas--)| Indicates whether the data are formulas. |
| [setIsFormulas(boolean[])](#setIsFormulas-booleanarray-)| Indicates whether the data are formulas. |
| [getTotalRows()](#getTotalRows--)| Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [setTotalRows(number)](#setTotalRows-number-)| Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [getTotalColumns()](#getTotalColumns--)| Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [setTotalColumns(number)](#setTotalColumns-number-)| Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [getColumnIndexes()](#getColumnIndexes--)| Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [setColumnIndexes(number[])](#setColumnIndexes-numberarray-)| Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [getDefaultValues()](#getDefaultValues--)| Default value for the value in the table is null. |
| [setDefaultValues(Object[])](#setDefaultValues-objectarray-)| Default value for the value in the table is null. |
| [isHtmlString()](#isHtmlString--)| Indicates whether the value contains html tags. |
| [setIsHtmlString(boolean)](#setIsHtmlString-boolean-)| Indicates whether the value contains html tags. |
| [getCheckMergedCells()](#getCheckMergedCells--)| Indicates whether checking merged cells. |
| [setCheckMergedCells(boolean)](#setCheckMergedCells-boolean-)| Indicates whether checking merged cells. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Creates the default importing options.

```javascript
constructor();
```


### getConvertGridStyle() {#getConvertGridStyle--}

Indicates whether apply the style of the grid view to cells.

```javascript
getConvertGridStyle() : boolean;
```


### setConvertGridStyle(boolean) {#setConvertGridStyle-boolean-}

Indicates whether apply the style of the grid view to cells.

```javascript
setConvertGridStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getConvertNumericData() {#getConvertNumericData--}

Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```javascript
getConvertNumericData() : boolean;
```


### setConvertNumericData(boolean) {#setConvertNumericData-boolean-}

Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```javascript
setConvertNumericData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getInsertRows() {#getInsertRows--}

Indicates whether new rows should be added for importing data records.

```javascript
getInsertRows() : boolean;
```


### setInsertRows(boolean) {#setInsertRows-boolean-}

Indicates whether new rows should be added for importing data records.

```javascript
setInsertRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShiftFirstRowDown() {#getShiftFirstRowDown--}

Indicates whether shifting the first row down when inserting rows.

```javascript
getShiftFirstRowDown() : boolean;
```


### setShiftFirstRowDown(boolean) {#setShiftFirstRowDown-boolean-}

Indicates whether shifting the first row down when inserting rows.

```javascript
setShiftFirstRowDown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFieldNameShown() {#isFieldNameShown--}

Indicates whether field name should be imported.

```javascript
isFieldNameShown() : boolean;
```


### setIsFieldNameShown(boolean) {#setIsFieldNameShown-boolean-}

Indicates whether field name should be imported.

```javascript
setIsFieldNameShown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}

Indicates whether exporting caption as field name

```javascript
getExportCaptionAsFieldName() : boolean;
```


**Remarks**

Only works for DataTable.

### setExportCaptionAsFieldName(boolean) {#setExportCaptionAsFieldName-boolean-}

Indicates whether exporting caption as field name

```javascript
setExportCaptionAsFieldName(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only works for DataTable.

### getDateFormat() {#getDateFormat--}

Gets or sets date format string for cells with imported datetime values.

```javascript
getDateFormat() : string;
```


### setDateFormat(string) {#setDateFormat-string-}

Gets or sets date format string for cells with imported datetime values.

```javascript
setDateFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNumberFormats() {#getNumberFormats--}

Gets or sets the number formats

```javascript
getNumberFormats() : string[];
```


**Returns**

string[]

### setNumberFormats(string[]) {#setNumberFormats-stringarray-}

Gets or sets the number formats

```javascript
setNumberFormats(value: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |

### getIsFormulas() {#getIsFormulas--}

Indicates whether the data are formulas.

```javascript
getIsFormulas() : boolean[];
```


**Returns**

boolean[]

### setIsFormulas(boolean[]) {#setIsFormulas-booleanarray-}

Indicates whether the data are formulas.

```javascript
setIsFormulas(value: boolean[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean[] | The value to set. |

### getTotalRows() {#getTotalRows--}

Gets or sets total row count to import from data source. -1 means all rows of given data source.

```javascript
getTotalRows() : number;
```


### setTotalRows(number) {#setTotalRows-number-}

Gets or sets total row count to import from data source. -1 means all rows of given data source.

```javascript
setTotalRows(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTotalColumns() {#getTotalColumns--}

Gets or sets total column count to import from data source. -1 means all rows of given data source.

```javascript
getTotalColumns() : number;
```


### setTotalColumns(number) {#setTotalColumns-number-}

Gets or sets total column count to import from data source. -1 means all rows of given data source.

```javascript
setTotalColumns(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnIndexes() {#getColumnIndexes--}

Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```javascript
getColumnIndexes() : number[];
```


**Returns**

number[]

### setColumnIndexes(number[]) {#setColumnIndexes-numberarray-}

Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```javascript
setColumnIndexes(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getDefaultValues() {#getDefaultValues--}

Default value for the value in the table is null.

```javascript
getDefaultValues() : Object[];
```


**Returns**

Object[]

### setDefaultValues(Object[]) {#setDefaultValues-objectarray-}

Default value for the value in the table is null.

```javascript
setDefaultValues(value: Object[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object[] | The value to set. |

### isHtmlString() {#isHtmlString--}

Indicates whether the value contains html tags.

```javascript
isHtmlString() : boolean;
```


### setIsHtmlString(boolean) {#setIsHtmlString-boolean-}

Indicates whether the value contains html tags.

```javascript
setIsHtmlString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCheckMergedCells() {#getCheckMergedCells--}

Indicates whether checking merged cells.

```javascript
getCheckMergedCells() : boolean;
```


### setCheckMergedCells(boolean) {#setCheckMergedCells-boolean-}

Indicates whether checking merged cells.

```javascript
setCheckMergedCells(value: boolean) : void;
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



