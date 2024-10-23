---
title: DataSorter
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Summary description for DataSorter.
type: docs
url: /nodejs-cpp/datasorter/
---

## DataSorter class

Summary description for DataSorter.

```javascript
class DataSorter;
```


### Example
```javascript
const { Workbook, CellArea, SortOrder } = require("aspose.cells.node");

//Instantiate a new Workbook object.
var workbook = new Workbook("input/DataSorter.xls");
//Get the workbook datasorter object.
var sorter = workbook.getDataSorter();
//Set the first order for datasorter object.
sorter.setOrder1(SortOrder.Descending);
//Define the first key.
sorter.setKey1(0);
//Create a cells area (range).
var ca = new CellArea();
//Specify the start row index.
ca.startRow = 0;
//Specify the start column index.
ca.startColumn = 0;
//Specify the last row index.
ca.endRow = 12;
//Specify the last column index.
ca.endColumn = 1;
//Sort data in the specified data range (A1:B14)
sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
//Save the excel file.
workbook.save("output/DataSorter.xls");
```
## Methods

| Method | Description |
| --- | --- |
| [getKeys()](#getKeys--)| Gets the key list of data sorter. |
| [getHasHeaders()](#getHasHeaders--)| Represents whether the range has headers. |
| [setHasHeaders(boolean)](#setHasHeaders-boolean-)| Represents whether the range has headers. |
| [getKey1()](#getKey1--)| Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey1(number)](#setKey1-number-)| Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder1()](#getOrder1--)| Represents sort order of the first key. |
| [setOrder1(SortOrder)](#setOrder1-sortorder-)| Represents sort order of the first key. |
| [getKey2()](#getKey2--)| Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey2(number)](#setKey2-number-)| Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder2()](#getOrder2--)| Represents sort order of the second key. |
| [setOrder2(SortOrder)](#setOrder2-sortorder-)| Represents sort order of the second key. |
| [getKey3()](#getKey3--)| Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [setKey3(number)](#setKey3-number-)| Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getOrder3()](#getOrder3--)| Represents sort order of the third key. |
| [setOrder3(SortOrder)](#setOrder3-sortorder-)| Represents sort order of the third key. |
| [getSortLeftToRight()](#getSortLeftToRight--)| True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [setSortLeftToRight(boolean)](#setSortLeftToRight-boolean-)| True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false. |
| [getCaseSensitive()](#getCaseSensitive--)| Gets and sets whether case sensitive when comparing string. |
| [setCaseSensitive(boolean)](#setCaseSensitive-boolean-)| Gets and sets whether case sensitive when comparing string. |
| [getSortAsNumber()](#getSortAsNumber--)| Indicates whether sorting anything that looks like a number. |
| [setSortAsNumber(boolean)](#setSortAsNumber-boolean-)| Indicates whether sorting anything that looks like a number. |
| [clear()](#clear--)| Clear all settings. |
| [addKey(number, SortOrder)](#addKey-number-sortorder-)| Adds sorted column index and sort order. |
| [addKey(number, SortOrder, string)](#addKey-number-sortorder-string-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOnType, SortOrder, object)](#addKey-number-sortontype-sortorder-object-)| Adds sorted column index and sort order with custom sort list. |
| [addKey(number, SortOrder, string[])](#addKey-number-sortorder-stringarray-)| Adds sorted column index and sort order with custom sort list. |
| [sort(Cells, number, number, number, number)](#sort-cells-number-number-number-number-)| Sorts the data of the area. |
| [sort(Cells, CellArea)](#sort-cells-cellarea-)| Sort the data of the area. |
| [sort()](#sort--)| Sort the data in the range. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### getKeys() {#getKeys--}

Gets the key list of data sorter.

```javascript
getKeys() : DataSorterKeyCollection;
```


**Returns**

[DataSorterKeyCollection](../datasorterkeycollection/)

### getHasHeaders() {#getHasHeaders--}

Represents whether the range has headers.

```javascript
getHasHeaders() : boolean;
```


### setHasHeaders(boolean) {#setHasHeaders-boolean-}

Represents whether the range has headers.

```javascript
setHasHeaders(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getKey1() {#getKey1--}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
getKey1() : number;
```


### setKey1(number) {#setKey1-number-}

Represents first sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
setKey1(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOrder1() {#getOrder1--}

Represents sort order of the first key.

```javascript
getOrder1() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### setOrder1(SortOrder) {#setOrder1-sortorder-}

Represents sort order of the first key.

```javascript
setOrder1(value: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |

### getKey2() {#getKey2--}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
getKey2() : number;
```


### setKey2(number) {#setKey2-number-}

Represents second sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
setKey2(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOrder2() {#getOrder2--}

Represents sort order of the second key.

```javascript
getOrder2() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### setOrder2(SortOrder) {#setOrder2-sortorder-}

Represents sort order of the second key.

```javascript
setOrder2(value: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |

### getKey3() {#getKey3--}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
getKey3() : number;
```


### setKey3(number) {#setKey3-number-}

Represents third sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
setKey3(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getOrder3() {#getOrder3--}

Represents sort order of the third key.

```javascript
getOrder3() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### setOrder3(SortOrder) {#setOrder3-sortorder-}

Represents sort order of the third key.

```javascript
setOrder3(value: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SortOrder](../sortorder/) | The value to set. |

### getSortLeftToRight() {#getSortLeftToRight--}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```javascript
getSortLeftToRight() : boolean;
```


### setSortLeftToRight(boolean) {#setSortLeftToRight-boolean-}

True means that sorting orientation is from left to right. False means that sorting orientation is from top to bottom. The default value is false.

```javascript
setSortLeftToRight(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getCaseSensitive() {#getCaseSensitive--}

Gets and sets whether case sensitive when comparing string.

```javascript
getCaseSensitive() : boolean;
```


### setCaseSensitive(boolean) {#setCaseSensitive-boolean-}

Gets and sets whether case sensitive when comparing string.

```javascript
setCaseSensitive(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getSortAsNumber() {#getSortAsNumber--}

Indicates whether sorting anything that looks like a number.

```javascript
getSortAsNumber() : boolean;
```


### setSortAsNumber(boolean) {#setSortAsNumber-boolean-}

Indicates whether sorting anything that looks like a number.

```javascript
setSortAsNumber(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### clear() {#clear--}

Clear all settings.

```javascript
clear() : void;
```


### addKey(number, SortOrder) {#addKey-number-sortorder-}

Adds sorted column index and sort order.

```javascript
addKey(key: number, order: SortOrder) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order |

### addKey(number, SortOrder, string) {#addKey-number-sortorder-string-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, order: SortOrder, customList: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string | The custom sort list. |

### addKey(number, SortOnType, SortOrder, object) {#addKey-number-sortontype-sortorder-object-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, type: SortOnType, order: SortOrder, customList: object) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| type | [SortOnType](../sortontype/) | The sorted value type. |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | object | The custom sort list. |

**Remarks**

If type is SortOnType.CellColor or SortOnType.FontColor, the customList is Color.

### addKey(number, SortOrder, string[]) {#addKey-number-sortorder-stringarray-}

Adds sorted column index and sort order with custom sort list.

```javascript
addKey(key: number, order: SortOrder, customList: string[]) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| key | number | The sorted column index(absolute position, column A is 0, B is 1, ...) |
| order | [SortOrder](../sortorder/) | The sort order. |
| customList | string[] | The custom sort list. |

### sort(Cells, number, number, number, number) {#sort-cells-number-number-number-number-}

Sorts the data of the area.

```javascript
sort(cells: Cells, startRow: number, startColumn: number, endRow: number, endColumn: number) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| startRow | number | The start row of the area. |
| startColumn | number | The start column of the area. |
| endRow | number | The end row of the area. |
| endColumn | number | The end column of the area. |

**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort(Cells, CellArea) {#sort-cells-cellarea-}

Sort the data of the area.

```javascript
sort(cells: Cells, area: CellArea) : number[];
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cells | [Cells](../cells/) | The cells contains the data area. |
| area | [CellArea](../cellarea/) | The area needed to sort |

**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### sort() {#sort--}

Sort the data in the range.

```javascript
sort() : number[];
```


**Returns**

the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns. If no rows/columns needs to be moved by this sorting operation, null will be returned.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



