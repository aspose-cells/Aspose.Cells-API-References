---
title: PivotTableCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the collection of all the PivotTable objects on the specified worksheet.
type: docs
url: /javascript-cpp/pivottablecollection/
---

## PivotTableCollection class

Represents the collection of all the PivotTable objects on the specified worksheet.

```javascript
class PivotTableCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotTable report by index. |
| [get(string)](#get-string-)| Gets the PivotTable report by pivottable's name. |
| [get(number, number)](#get-number-number-)| Gets the PivotTable report by pivottable's position. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [add(string, string, string)](#add-string-string-string-)| Adds a new PivotTable. |
| [add(string, string, string, boolean)](#add-string-string-string-boolean-)| Adds a new PivotTable. |
| [add(string, number, number, string)](#add-string-number-number-string-)| Adds a new PivotTable. |
| [add(string, number, number, string, boolean)](#add-string-number-number-string-boolean-)| Adds a new PivotTable. |
| [add(string, number, number, string, boolean, boolean)](#add-string-number-number-string-boolean-boolean-)| Adds a new PivotTable. |
| [add(string, string, string, boolean, boolean)](#add-string-string-string-boolean-boolean-)| Adds a new PivotTable. |
| [add(PivotTable, string, string)](#add-pivottable-string-string-)| Adds a new PivotTable based on another PivotTable. |
| [add(PivotTable, number, number, string)](#add-pivottable-number-number-string-)| Adds a new PivotTable based on another PivotTable. |
| [add(string[], boolean, PivotPageFields, string, string)](#add-stringarray-boolean-pivotpagefields-string-string-)| Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [add(string[], boolean, PivotPageFields, number, number, string)](#add-stringarray-boolean-pivotpagefields-number-number-string-)| Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source. |
| [clear()](#clear--)| Clears all pivot tables. |
| [remove(PivotTable)](#remove-pivottable-)| Deletes the specified PivotTable and delete the PivotTable data |
| [remove(PivotTable, boolean)](#remove-pivottable-boolean-)| Deletes the specified PivotTable |
| [removeAt(number)](#removeAt-number-)| Deletes the PivotTable at the specified index and delete the PivotTable data |
| [removeAt(number, boolean)](#removeAt-number-boolean-)| Deletes the PivotTable at the specified index |


### get(number) {#get-number-}

Gets the PivotTable report by index.

```javascript
get(index: number) : PivotTable;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotTable](../pivottable/)

### get(string) {#get-string-}

Gets the PivotTable report by pivottable's name.

```javascript
get(name: string) : PivotTable;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| name | string |  |

**Returns**

[PivotTable](../pivottable/)

### get(number, number) {#get-number-number-}

Gets the PivotTable report by pivottable's position.

```javascript
get(row: number, column: number) : PivotTable;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number |  |
| column | number |  |

**Returns**

[PivotTable](../pivottable/)

### dispose() {#dispose--}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```javascript
dispose() : void;
```


### add(string, string, string) {#add-string-string-string-}

Adds a new PivotTable.

```javascript
add(sourceData: string, destCellName: string, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data for the new PivotTable cache. |
| destCellName | string | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |

**Returns**

The new added cache index.

### add(string, string, string, boolean) {#add-string-string-string-boolean-}

Adds a new PivotTable.

```javascript
add(sourceData: string, destCellName: string, tableName: string, useSameSource: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data for the new PivotTable cache. |
| destCellName | string | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source.         /// If the property is true, it will save memory. |

**Returns**

The new added cache index.

### add(string, number, number, string) {#add-string-number-number-string-}

Adds a new PivotTable.

```javascript
add(sourceData: string, row: number, column: number, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |

**Returns**

The new added cache index.

### add(string, number, number, string, boolean) {#add-string-number-number-string-boolean-}

Adds a new PivotTable.

```javascript
add(sourceData: string, row: number, column: number, tableName: string, useSameSource: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source.         /// If the property is true, it will save memory. |

**Returns**

The new added cache index.

### add(string, number, number, string, boolean, boolean) {#add-string-number-number-string-boolean-boolean-}

Adds a new PivotTable.

```javascript
add(sourceData: string, row: number, column: number, tableName: string, useSameSource: boolean, isXlsClassic: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| row | number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source.         /// If the property is true, it will save memory. |
| isXlsClassic | boolean | Indicates whether add classic pivot table of Excel 97-2003. |

**Returns**

The new added cache index.

### add(string, string, string, boolean, boolean) {#add-string-string-string-boolean-boolean-}

Adds a new PivotTable.

```javascript
add(sourceData: string, cell: string, tableName: string, useSameSource: boolean, isXlsClassic: boolean) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string | The data cell range for the new PivotTable.Example : Sheet1!A1:C8 |
| cell | string | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |
| useSameSource | boolean | Indicates whether using same data source when another existing pivot table has used this data source.           /// If the property is true, it will save memory. |
| isXlsClassic | boolean | Indicates whether add classic pivot table of Excel 97-2003. |

**Returns**

The new added cache index.

### add(PivotTable, string, string) {#add-pivottable-string-string-}

Adds a new PivotTable based on another PivotTable.

```javascript
add(pivotTable: PivotTable, destCellName: string, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../pivottable/) | The source pivotTable. |
| destCellName | string | The cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |

**Returns**

The new added PivotTable index.

### add(PivotTable, number, number, string) {#add-pivottable-number-number-string-}

Adds a new PivotTable based on another PivotTable.

```javascript
add(pivotTable: PivotTable, row: number, column: number, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../pivottable/) | The source pivotTable. |
| row | number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |

**Returns**

The new added PivotTable index.

### add(string[], boolean, PivotPageFields, string, string) {#add-stringarray-boolean-pivotpagefields-string-string-}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```javascript
add(sourceData: string[], isAutoPage: boolean, pageFields: PivotPageFields, destCellName: string, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field.         /// If true,the following param pageFields will be ignored. |
| pageFields | [PivotPageFields](../pivotpagefields/) | The pivot page field items. |
| destCellName | string | destCellName The name of the new PivotTable report. |
| tableName | string | the name of the new PivotTable report. |

**Returns**

The new added PivotTable index.

### add(string[], boolean, PivotPageFields, number, number, string) {#add-stringarray-boolean-pivotpagefields-number-number-string-}

Adds a new PivotTable Object to the collection with multiple consolidation ranges as data source.

```javascript
add(sourceData: string[], isAutoPage: boolean, pageFields: PivotPageFields, row: number, column: number, tableName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceData | string[] | The multiple consolidation ranges,such as {"Sheet1!A1:C8","Sheet2!A1:B8"} |
| isAutoPage | boolean | Whether auto create a single page field.         /// If true,the following param pageFields will be ignored |
| pageFields | [PivotPageFields](../pivotpagefields/) | The pivot page field items. |
| row | number | Row index of the cell in the upper-left corner of the PivotTable report's destination range. |
| column | number | Column index of the cell in the upper-left corner of the PivotTable report's destination range. |
| tableName | string | The name of the new PivotTable report. |

**Returns**

The new added PivotTable index.

### clear() {#clear--}

Clears all pivot tables.

```javascript
clear() : void;
```


### remove(PivotTable) {#remove-pivottable-}

Deletes the specified PivotTable and delete the PivotTable data

```javascript
remove(pivotTable: PivotTable) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../pivottable/) | PivotTable object |

### remove(PivotTable, boolean) {#remove-pivottable-boolean-}

Deletes the specified PivotTable

```javascript
remove(pivotTable: PivotTable, keepData: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivotTable | [PivotTable](../pivottable/) | PivotTable object |
| keepData | boolean | Whether to keep the PivotTable data |

### removeAt(number) {#removeAt-number-}

Deletes the PivotTable at the specified index and delete the PivotTable data

```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the position index in PivotTable collection |

### removeAt(number, boolean) {#removeAt-number-boolean-}

Deletes the PivotTable at the specified index

```javascript
removeAt(index: number, keepData: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the position index in PivotTable collection |
| keepData | boolean | Whether to keep the PivotTable data |


