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

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Creates the default importing options. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [convertGridStyle](#convertGridStyle--)| boolean | Indicates whether apply the style of the grid view to cells. |
| [convertNumericData](#convertNumericData--)| boolean | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [insertRows](#insertRows--)| boolean | Indicates whether new rows should be added for importing data records. |
| [shiftFirstRowDown](#shiftFirstRowDown--)| boolean | Indicates whether shifting the first row down when inserting rows. |
| [isFieldNameShown](#isFieldNameShown--)| boolean | Indicates whether field name should be imported. |
| [exportCaptionAsFieldName](#exportCaptionAsFieldName--)| boolean | Indicates whether exporting caption as field name |
| [dateFormat](#dateFormat--)| string | Gets or sets date format string for cells with imported datetime values. |
| [numberFormats](#numberFormats--)| string[] | Gets or sets the number formats |
| [styles](#styles--)| Style[] | Gets and sets the styles for each column of the table. |
| [isFormulas](#isFormulas--)| boolean[] | Indicates whether the data are formulas. |
| [totalRows](#totalRows--)| number | Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [totalColumns](#totalColumns--)| number | Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [columnIndexes](#columnIndexes--)| number[] | Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [defaultValues](#defaultValues--)| Object[] | Default value for the value in the table is null. |
| [isHtmlString](#isHtmlString--)| boolean | Indicates whether the value contains html tags. |
| [checkMergedCells](#checkMergedCells--)| boolean | Indicates whether checking merged cells. |

## Methods

| Method | Description |
| --- | --- |
| [getConvertGridStyle()](#getConvertGridStyle--)| <b>@deprecated.</b> Please use the 'convertGridStyle' property instead. Indicates whether apply the style of the grid view to cells. |
| [setConvertGridStyle(boolean)](#setConvertGridStyle-boolean-)| <b>@deprecated.</b> Please use the 'convertGridStyle' property instead. Indicates whether apply the style of the grid view to cells. |
| [getConvertNumericData()](#getConvertNumericData--)| <b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [setConvertNumericData(boolean)](#setConvertNumericData-boolean-)| <b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string value should be converted to numeric or date value. |
| [getInsertRows()](#getInsertRows--)| <b>@deprecated.</b> Please use the 'insertRows' property instead. Indicates whether new rows should be added for importing data records. |
| [setInsertRows(boolean)](#setInsertRows-boolean-)| <b>@deprecated.</b> Please use the 'insertRows' property instead. Indicates whether new rows should be added for importing data records. |
| [getShiftFirstRowDown()](#getShiftFirstRowDown--)| <b>@deprecated.</b> Please use the 'shiftFirstRowDown' property instead. Indicates whether shifting the first row down when inserting rows. |
| [setShiftFirstRowDown(boolean)](#setShiftFirstRowDown-boolean-)| <b>@deprecated.</b> Please use the 'shiftFirstRowDown' property instead. Indicates whether shifting the first row down when inserting rows. |
| [isFieldNameShown()](#isFieldNameShown--)| <b>@deprecated.</b> Please use the 'isFieldNameShown' property instead. Indicates whether field name should be imported. |
| [setIsFieldNameShown(boolean)](#setIsFieldNameShown-boolean-)| <b>@deprecated.</b> Please use the 'isFieldNameShown' property instead. Indicates whether field name should be imported. |
| [getExportCaptionAsFieldName()](#getExportCaptionAsFieldName--)| <b>@deprecated.</b> Please use the 'exportCaptionAsFieldName' property instead. Indicates whether exporting caption as field name |
| [setExportCaptionAsFieldName(boolean)](#setExportCaptionAsFieldName-boolean-)| <b>@deprecated.</b> Please use the 'exportCaptionAsFieldName' property instead. Indicates whether exporting caption as field name |
| [getDateFormat()](#getDateFormat--)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets or sets date format string for cells with imported datetime values. |
| [setDateFormat(string)](#setDateFormat-string-)| <b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets or sets date format string for cells with imported datetime values. |
| [getNumberFormats()](#getNumberFormats--)| <b>@deprecated.</b> Please use the 'numberFormats' property instead. Gets or sets the number formats |
| [setNumberFormats(string[])](#setNumberFormats-stringarray-)| <b>@deprecated.</b> Please use the 'numberFormats' property instead. Gets or sets the number formats |
| [getStyles()](#getStyles--)| <b>@deprecated.</b> Please use the 'styles' property instead. Gets and sets the styles for each column of the table. |
| [setStyles(Style[])](#setStyles-stylearray-)| <b>@deprecated.</b> Please use the 'styles' property instead. Gets and sets the styles for each column of the table. |
| [getIsFormulas()](#getIsFormulas--)| <b>@deprecated.</b> Please use the 'isFormulas' property instead. Indicates whether the data are formulas. |
| [setIsFormulas(boolean[])](#setIsFormulas-booleanarray-)| <b>@deprecated.</b> Please use the 'isFormulas' property instead. Indicates whether the data are formulas. |
| [getTotalRows()](#getTotalRows--)| <b>@deprecated.</b> Please use the 'totalRows' property instead. Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [setTotalRows(number)](#setTotalRows-number-)| <b>@deprecated.</b> Please use the 'totalRows' property instead. Gets or sets total row count to import from data source. -1 means all rows of given data source. |
| [getTotalColumns()](#getTotalColumns--)| <b>@deprecated.</b> Please use the 'totalColumns' property instead. Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [setTotalColumns(number)](#setTotalColumns-number-)| <b>@deprecated.</b> Please use the 'totalColumns' property instead. Gets or sets total column count to import from data source. -1 means all rows of given data source. |
| [getColumnIndexes()](#getColumnIndexes--)| <b>@deprecated.</b> Please use the 'columnIndexes' property instead. Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [setColumnIndexes(number[])](#setColumnIndexes-numberarray-)| <b>@deprecated.</b> Please use the 'columnIndexes' property instead. Gets or sets the columns(0-based) to import from data source. null means all columns should be imported. |
| [getDefaultValues()](#getDefaultValues--)| <b>@deprecated.</b> Please use the 'defaultValues' property instead. Default value for the value in the table is null. |
| [setDefaultValues(Object[])](#setDefaultValues-objectarray-)| <b>@deprecated.</b> Please use the 'defaultValues' property instead. Default value for the value in the table is null. |
| [isHtmlString()](#isHtmlString--)| <b>@deprecated.</b> Please use the 'isHtmlString' property instead. Indicates whether the value contains html tags. |
| [setIsHtmlString(boolean)](#setIsHtmlString-boolean-)| <b>@deprecated.</b> Please use the 'isHtmlString' property instead. Indicates whether the value contains html tags. |
| [getCheckMergedCells()](#getCheckMergedCells--)| <b>@deprecated.</b> Please use the 'checkMergedCells' property instead. Indicates whether checking merged cells. |
| [setCheckMergedCells(boolean)](#setCheckMergedCells-boolean-)| <b>@deprecated.</b> Please use the 'checkMergedCells' property instead. Indicates whether checking merged cells. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Creates the default importing options.

```javascript
constructor();
```


### convertGridStyle {#convertGridStyle--}

Indicates whether apply the style of the grid view to cells.

```javascript
convertGridStyle : boolean;
```


### convertNumericData {#convertNumericData--}

Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```javascript
convertNumericData : boolean;
```


### insertRows {#insertRows--}

Indicates whether new rows should be added for importing data records.

```javascript
insertRows : boolean;
```


### shiftFirstRowDown {#shiftFirstRowDown--}

Indicates whether shifting the first row down when inserting rows.

```javascript
shiftFirstRowDown : boolean;
```


### isFieldNameShown {#isFieldNameShown--}

Indicates whether field name should be imported.

```javascript
isFieldNameShown : boolean;
```


### exportCaptionAsFieldName {#exportCaptionAsFieldName--}

Indicates whether exporting caption as field name

```javascript
exportCaptionAsFieldName : boolean;
```


**Remarks**

Only works for DataTable.

### dateFormat {#dateFormat--}

Gets or sets date format string for cells with imported datetime values.

```javascript
dateFormat : string;
```


### numberFormats {#numberFormats--}

Gets or sets the number formats

```javascript
numberFormats : string[];
```


### styles {#styles--}

Gets and sets the styles for each column of the table.

```javascript
styles : Style[];
```


### isFormulas {#isFormulas--}

Indicates whether the data are formulas.

```javascript
isFormulas : boolean[];
```


### totalRows {#totalRows--}

Gets or sets total row count to import from data source. -1 means all rows of given data source.

```javascript
totalRows : number;
```


### totalColumns {#totalColumns--}

Gets or sets total column count to import from data source. -1 means all rows of given data source.

```javascript
totalColumns : number;
```


### columnIndexes {#columnIndexes--}

Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```javascript
columnIndexes : number[];
```


### defaultValues {#defaultValues--}

Default value for the value in the table is null.

```javascript
defaultValues : Object[];
```


### isHtmlString {#isHtmlString--}

Indicates whether the value contains html tags.

```javascript
isHtmlString : boolean;
```


### checkMergedCells {#checkMergedCells--}

Indicates whether checking merged cells.

```javascript
checkMergedCells : boolean;
```


### getConvertGridStyle() {#getConvertGridStyle--}

<b>@deprecated.</b> Please use the 'convertGridStyle' property instead. Indicates whether apply the style of the grid view to cells.

```javascript
getConvertGridStyle() : boolean;
```


### setConvertGridStyle(boolean) {#setConvertGridStyle-boolean-}

<b>@deprecated.</b> Please use the 'convertGridStyle' property instead. Indicates whether apply the style of the grid view to cells.

```javascript
setConvertGridStyle(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getConvertNumericData() {#getConvertNumericData--}

<b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```javascript
getConvertNumericData() : boolean;
```


### setConvertNumericData(boolean) {#setConvertNumericData-boolean-}

<b>@deprecated.</b> Please use the 'convertNumericData' property instead. Gets or sets a value that indicates whether the string value should be converted to numeric or date value.

```javascript
setConvertNumericData(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getInsertRows() {#getInsertRows--}

<b>@deprecated.</b> Please use the 'insertRows' property instead. Indicates whether new rows should be added for importing data records.

```javascript
getInsertRows() : boolean;
```


### setInsertRows(boolean) {#setInsertRows-boolean-}

<b>@deprecated.</b> Please use the 'insertRows' property instead. Indicates whether new rows should be added for importing data records.

```javascript
setInsertRows(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShiftFirstRowDown() {#getShiftFirstRowDown--}

<b>@deprecated.</b> Please use the 'shiftFirstRowDown' property instead. Indicates whether shifting the first row down when inserting rows.

```javascript
getShiftFirstRowDown() : boolean;
```


### setShiftFirstRowDown(boolean) {#setShiftFirstRowDown-boolean-}

<b>@deprecated.</b> Please use the 'shiftFirstRowDown' property instead. Indicates whether shifting the first row down when inserting rows.

```javascript
setShiftFirstRowDown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFieldNameShown() {#isFieldNameShown--}

<b>@deprecated.</b> Please use the 'isFieldNameShown' property instead. Indicates whether field name should be imported.

```javascript
isFieldNameShown() : boolean;
```


### setIsFieldNameShown(boolean) {#setIsFieldNameShown-boolean-}

<b>@deprecated.</b> Please use the 'isFieldNameShown' property instead. Indicates whether field name should be imported.

```javascript
setIsFieldNameShown(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getExportCaptionAsFieldName() {#getExportCaptionAsFieldName--}

<b>@deprecated.</b> Please use the 'exportCaptionAsFieldName' property instead. Indicates whether exporting caption as field name

```javascript
getExportCaptionAsFieldName() : boolean;
```


**Remarks**

Only works for DataTable.

### setExportCaptionAsFieldName(boolean) {#setExportCaptionAsFieldName-boolean-}

<b>@deprecated.</b> Please use the 'exportCaptionAsFieldName' property instead. Indicates whether exporting caption as field name

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

<b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets or sets date format string for cells with imported datetime values.

```javascript
getDateFormat() : string;
```


### setDateFormat(string) {#setDateFormat-string-}

<b>@deprecated.</b> Please use the 'dateFormat' property instead. Gets or sets date format string for cells with imported datetime values.

```javascript
setDateFormat(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getNumberFormats() {#getNumberFormats--}

<b>@deprecated.</b> Please use the 'numberFormats' property instead. Gets or sets the number formats

```javascript
getNumberFormats() : string[];
```


**Returns**

string[]

### setNumberFormats(string[]) {#setNumberFormats-stringarray-}

<b>@deprecated.</b> Please use the 'numberFormats' property instead. Gets or sets the number formats

```javascript
setNumberFormats(value: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string[] | The value to set. |

### getStyles() {#getStyles--}

<b>@deprecated.</b> Please use the 'styles' property instead. Gets and sets the styles for each column of the table.

```javascript
getStyles() : Style[];
```


**Returns**

[Style](../style/)[]

### setStyles(Style[]) {#setStyles-stylearray-}

<b>@deprecated.</b> Please use the 'styles' property instead. Gets and sets the styles for each column of the table.

```javascript
setStyles(value: Style[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/)[] | The value to set. |

### getIsFormulas() {#getIsFormulas--}

<b>@deprecated.</b> Please use the 'isFormulas' property instead. Indicates whether the data are formulas.

```javascript
getIsFormulas() : boolean[];
```


**Returns**

boolean[]

### setIsFormulas(boolean[]) {#setIsFormulas-booleanarray-}

<b>@deprecated.</b> Please use the 'isFormulas' property instead. Indicates whether the data are formulas.

```javascript
setIsFormulas(value: boolean[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean[] | The value to set. |

### getTotalRows() {#getTotalRows--}

<b>@deprecated.</b> Please use the 'totalRows' property instead. Gets or sets total row count to import from data source. -1 means all rows of given data source.

```javascript
getTotalRows() : number;
```


### setTotalRows(number) {#setTotalRows-number-}

<b>@deprecated.</b> Please use the 'totalRows' property instead. Gets or sets total row count to import from data source. -1 means all rows of given data source.

```javascript
setTotalRows(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTotalColumns() {#getTotalColumns--}

<b>@deprecated.</b> Please use the 'totalColumns' property instead. Gets or sets total column count to import from data source. -1 means all rows of given data source.

```javascript
getTotalColumns() : number;
```


### setTotalColumns(number) {#setTotalColumns-number-}

<b>@deprecated.</b> Please use the 'totalColumns' property instead. Gets or sets total column count to import from data source. -1 means all rows of given data source.

```javascript
setTotalColumns(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getColumnIndexes() {#getColumnIndexes--}

<b>@deprecated.</b> Please use the 'columnIndexes' property instead. Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```javascript
getColumnIndexes() : number[];
```


**Returns**

number[]

### setColumnIndexes(number[]) {#setColumnIndexes-numberarray-}

<b>@deprecated.</b> Please use the 'columnIndexes' property instead. Gets or sets the columns(0-based) to import from data source. null means all columns should be imported.

```javascript
setColumnIndexes(value: number[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |

### getDefaultValues() {#getDefaultValues--}

<b>@deprecated.</b> Please use the 'defaultValues' property instead. Default value for the value in the table is null.

```javascript
getDefaultValues() : Object[];
```


**Returns**

Object[]

### setDefaultValues(Object[]) {#setDefaultValues-objectarray-}

<b>@deprecated.</b> Please use the 'defaultValues' property instead. Default value for the value in the table is null.

```javascript
setDefaultValues(value: Object[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object[] | The value to set. |

### isHtmlString() {#isHtmlString--}

<b>@deprecated.</b> Please use the 'isHtmlString' property instead. Indicates whether the value contains html tags.

```javascript
isHtmlString() : boolean;
```


### setIsHtmlString(boolean) {#setIsHtmlString-boolean-}

<b>@deprecated.</b> Please use the 'isHtmlString' property instead. Indicates whether the value contains html tags.

```javascript
setIsHtmlString(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCheckMergedCells() {#getCheckMergedCells--}

<b>@deprecated.</b> Please use the 'checkMergedCells' property instead. Indicates whether checking merged cells.

```javascript
getCheckMergedCells() : boolean;
```


### setCheckMergedCells(boolean) {#setCheckMergedCells-boolean-}

<b>@deprecated.</b> Please use the 'checkMergedCells' property instead. Indicates whether checking merged cells.

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



