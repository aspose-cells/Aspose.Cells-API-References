---
title: ListObject
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.
type: docs
url: /nodejs-cpp/listobject/
---

## ListObject class

Represents a list object on a worksheet. The ListObject object is a member of the ListObjects collection. The ListObjects collection contains all the list objects on a worksheet.

```javascript
class ListObject;
```


## Methods

| Method | Description |
| --- | --- |
| [getStartRow()](#getStartRow--)| Gets the start row of the range. |
| [getStartColumn()](#getStartColumn--)| Gets the start column of the range. |
| [getEndRow()](#getEndRow--)| Gets the end  row of the range. |
| [getEndColumn()](#getEndColumn--)| Gets the end column of the range. |
| [getListColumns()](#getListColumns--)| Gets ListColumns of the ListObject. |
| [getShowHeaderRow()](#getShowHeaderRow--)| Gets and sets whether this ListObject show header row. |
| [setShowHeaderRow(boolean)](#setShowHeaderRow-boolean-)| Gets and sets whether this ListObject show header row. |
| [getShowTotals()](#getShowTotals--)| Gets and sets whether this ListObject show total row. |
| [setShowTotals(boolean)](#setShowTotals-boolean-)| Gets and sets whether this ListObject show total row. |
| [getDataRange()](#getDataRange--)| Gets the data range of the ListObject. |
| [getQueryTable()](#getQueryTable--)| Gets the linked QueryTable. |
| [getDataSourceType()](#getDataSourceType--)| Gets the data source type of the table. |
| [getAutoFilter()](#getAutoFilter--)| Gets auto filter. |
| [getDisplayName()](#getDisplayName--)| Gets and sets the display name. |
| [setDisplayName(string)](#setDisplayName-string-)| Gets and sets the display name. |
| [getComment()](#getComment--)| Gets and sets the comment of the table. |
| [setComment(string)](#setComment-string-)| Gets and sets the comment of the table. |
| [getShowTableStyleFirstColumn()](#getShowTableStyleFirstColumn--)| Indicates whether the first column in the table should have the style applied. |
| [setShowTableStyleFirstColumn(boolean)](#setShowTableStyleFirstColumn-boolean-)| Indicates whether the first column in the table should have the style applied. |
| [getShowTableStyleLastColumn()](#getShowTableStyleLastColumn--)| Indicates whether the last column in the table should have the style applied. |
| [setShowTableStyleLastColumn(boolean)](#setShowTableStyleLastColumn-boolean-)| Indicates whether the last column in the table should have the style applied. |
| [getShowTableStyleRowStripes()](#getShowTableStyleRowStripes--)| Indicates whether row stripe formatting is applied. |
| [setShowTableStyleRowStripes(boolean)](#setShowTableStyleRowStripes-boolean-)| Indicates whether row stripe formatting is applied. |
| [getShowTableStyleColumnStripes()](#getShowTableStyleColumnStripes--)| Indicates whether column stripe formatting is applied. |
| [setShowTableStyleColumnStripes(boolean)](#setShowTableStyleColumnStripes-boolean-)| Indicates whether column stripe formatting is applied. |
| [getTableStyleType()](#getTableStyleType--)| Gets and the built-in table style. |
| [setTableStyleType(TableStyleType)](#setTableStyleType-tablestyletype-)| Gets and the built-in table style. |
| [getTableStyleName()](#getTableStyleName--)| Gets and sets the table style name. |
| [setTableStyleName(string)](#setTableStyleName-string-)| Gets and sets the table style name. |
| [getXmlMap()](#getXmlMap--)| Gets an [XmlMap](/nodejs-cpp/xmlmap/) used for this list. |
| [getAlternativeText()](#getAlternativeText--)| Gets and sets the alternative text. |
| [setAlternativeText(string)](#setAlternativeText-string-)| Gets and sets the alternative text. |
| [getAlternativeDescription()](#getAlternativeDescription--)| Gets and sets the alternative description. |
| [setAlternativeDescription(string)](#setAlternativeDescription-string-)| Gets and sets the alternative description. |
| [resize(number, number, number, number, boolean)](#resize-number-number-number-number-boolean-)| Resize the range of the list object. |
| [putCellFormula(number, number, string)](#putCellFormula-number-number-string-)| Put the formula to the cell in the table. |
| [putCellFormula(number, number, string, boolean)](#putCellFormula-number-number-string-boolean-)| Put the formula to the cell in the table. |
| [updateColumnName()](#updateColumnName--)| Updates all list columns' name from the worksheet. |
| [filter()](#filter--)| Filter the table. |
| [applyStyleToRange()](#applyStyleToRange--)| Apply the table style to the range. |
| [convertToRange()](#convertToRange--)| Convert the table to range. |
| [convertToRange(TableToRangeOptions)](#convertToRange-tabletorangeoptions-)| Convert the table to range. |


### getStartRow() {#getStartRow--}

Gets the start row of the range.

```javascript
getStartRow() : number;
```


### getStartColumn() {#getStartColumn--}

Gets the start column of the range.

```javascript
getStartColumn() : number;
```


### getEndRow() {#getEndRow--}

Gets the end  row of the range.

```javascript
getEndRow() : number;
```


### getEndColumn() {#getEndColumn--}

Gets the end column of the range.

```javascript
getEndColumn() : number;
```


### getListColumns() {#getListColumns--}

Gets ListColumns of the ListObject.

```javascript
getListColumns() : ListColumnCollection;
```


**Returns**

[ListColumnCollection](/nodejs-cpp/listcolumncollection/)

### getShowHeaderRow() {#getShowHeaderRow--}

Gets and sets whether this ListObject show header row.

```javascript
getShowHeaderRow() : boolean;
```


### setShowHeaderRow(boolean) {#setShowHeaderRow-boolean-}

Gets and sets whether this ListObject show header row.

```javascript
setShowHeaderRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowTotals() {#getShowTotals--}

Gets and sets whether this ListObject show total row.

```javascript
getShowTotals() : boolean;
```


### setShowTotals(boolean) {#setShowTotals-boolean-}

Gets and sets whether this ListObject show total row.

```javascript
setShowTotals(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getDataRange() {#getDataRange--}

Gets the data range of the ListObject.

```javascript
getDataRange() : Range;
```


**Returns**

[Range](/nodejs-cpp/range/)

### getQueryTable() {#getQueryTable--}

Gets the linked QueryTable.

```javascript
getQueryTable() : QueryTable;
```


**Returns**

[QueryTable](/nodejs-cpp/querytable/)

### getDataSourceType() {#getDataSourceType--}

Gets the data source type of the table.

```javascript
getDataSourceType() : TableDataSourceType;
```


**Returns**

[TableDataSourceType](/nodejs-cpp/tabledatasourcetype/)

### getAutoFilter() {#getAutoFilter--}

Gets auto filter.

```javascript
getAutoFilter() : AutoFilter;
```


**Returns**

[AutoFilter](/nodejs-cpp/autofilter/)

### getDisplayName() {#getDisplayName--}

Gets and sets the display name.

```javascript
getDisplayName() : string;
```


### setDisplayName(string) {#setDisplayName-string-}

Gets and sets the display name.

```javascript
setDisplayName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getComment() {#getComment--}

Gets and sets the comment of the table.

```javascript
getComment() : string;
```


### setComment(string) {#setComment-string-}

Gets and sets the comment of the table.

```javascript
setComment(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getShowTableStyleFirstColumn() {#getShowTableStyleFirstColumn--}

Indicates whether the first column in the table should have the style applied.

```javascript
getShowTableStyleFirstColumn() : boolean;
```


### setShowTableStyleFirstColumn(boolean) {#setShowTableStyleFirstColumn-boolean-}

Indicates whether the first column in the table should have the style applied.

```javascript
setShowTableStyleFirstColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowTableStyleLastColumn() {#getShowTableStyleLastColumn--}

Indicates whether the last column in the table should have the style applied.

```javascript
getShowTableStyleLastColumn() : boolean;
```


### setShowTableStyleLastColumn(boolean) {#setShowTableStyleLastColumn-boolean-}

Indicates whether the last column in the table should have the style applied.

```javascript
setShowTableStyleLastColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowTableStyleRowStripes() {#getShowTableStyleRowStripes--}

Indicates whether row stripe formatting is applied.

```javascript
getShowTableStyleRowStripes() : boolean;
```


### setShowTableStyleRowStripes(boolean) {#setShowTableStyleRowStripes-boolean-}

Indicates whether row stripe formatting is applied.

```javascript
setShowTableStyleRowStripes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getShowTableStyleColumnStripes() {#getShowTableStyleColumnStripes--}

Indicates whether column stripe formatting is applied.

```javascript
getShowTableStyleColumnStripes() : boolean;
```


### setShowTableStyleColumnStripes(boolean) {#setShowTableStyleColumnStripes-boolean-}

Indicates whether column stripe formatting is applied.

```javascript
setShowTableStyleColumnStripes(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTableStyleType() {#getTableStyleType--}

Gets and the built-in table style.

```javascript
getTableStyleType() : TableStyleType;
```


**Returns**

[TableStyleType](/nodejs-cpp/tablestyletype/)

### setTableStyleType(TableStyleType) {#setTableStyleType-tablestyletype-}

Gets and the built-in table style.

```javascript
setTableStyleType(value: TableStyleType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TableStyleType](/nodejs-cpp/tablestyletype/) | The value to set. |

### getTableStyleName() {#getTableStyleName--}

Gets and sets the table style name.

```javascript
getTableStyleName() : string;
```


### setTableStyleName(string) {#setTableStyleName-string-}

Gets and sets the table style name.

```javascript
setTableStyleName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getXmlMap() {#getXmlMap--}

Gets an [XmlMap](/nodejs-cpp/xmlmap/) used for this list.

```javascript
getXmlMap() : XmlMap;
```


**Returns**

[XmlMap](/nodejs-cpp/xmlmap/)

### getAlternativeText() {#getAlternativeText--}

Gets and sets the alternative text.

```javascript
getAlternativeText() : string;
```


### setAlternativeText(string) {#setAlternativeText-string-}

Gets and sets the alternative text.

```javascript
setAlternativeText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAlternativeDescription() {#getAlternativeDescription--}

Gets and sets the alternative description.

```javascript
getAlternativeDescription() : string;
```


### setAlternativeDescription(string) {#setAlternativeDescription-string-}

Gets and sets the alternative description.

```javascript
setAlternativeDescription(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### resize(number, number, number, number, boolean) {#resize-number-number-number-number-boolean-}

Resize the range of the list object.

```javascript
resize(startRow: number, startColumn: number, endRow: number, endColumn: number, hasHeaders: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The start row index of the new range. |
| startColumn | number | The start column index of the new range. |
| endRow | number | The end row index of the new range. |
| endColumn | number | The end column index of the new range. |
| hasHeaders | boolean | Whether this table has headers. |

### putCellFormula(number, number, string) {#putCellFormula-number-number-string-}

Put the formula to the cell in the table.

```javascript
putCellFormula(rowOffset: number, columnOffset: number, formula: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| formula | string | The formula of the cell. |

### putCellFormula(number, number, string, boolean) {#putCellFormula-number-number-string-boolean-}

Put the formula to the cell in the table.

```javascript
putCellFormula(rowOffset: number, columnOffset: number, formula: string, isTotalsRowFormula: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowOffset | number | The row offset in the table. |
| columnOffset | number | The column offset in the table. |
| formula | string | The formula of the cell. |
| isTotalsRowFormula | boolean |  |

### updateColumnName() {#updateColumnName--}

Updates all list columns' name from the worksheet.

```javascript
updateColumnName() : void;
```


**Remarks**

The value of the cells in the header row of the table must be same as the name of the ListColumn; Cell.PutValue do not auto modify the name of the ListColumn for performance.

### filter() {#filter--}

Filter the table.

```javascript
filter() : AutoFilter;
```


**Returns**

[AutoFilter](/nodejs-cpp/autofilter/)

### applyStyleToRange() {#applyStyleToRange--}

Apply the table style to the range.

```javascript
applyStyleToRange() : void;
```


### convertToRange() {#convertToRange--}

Convert the table to range.

```javascript
convertToRange() : void;
```


### convertToRange(TableToRangeOptions) {#convertToRange-tabletorangeoptions-}

Convert the table to range.

```javascript
convertToRange(options: TableToRangeOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [TableToRangeOptions](/nodejs-cpp/tabletorangeoptions/) | the options when converting table to range. |


