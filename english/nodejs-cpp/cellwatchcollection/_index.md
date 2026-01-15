---
title: CellWatchCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the collection of cells on this worksheet being watched in the watch window.
type: docs
url: /nodejs-cpp/cellwatchcollection/
---

## CellWatchCollection class

Represents the collection of cells on this worksheet being watched in the 'watch window'.

```javascript
class CellWatchCollection;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets and sets [CellWatch](../cellwatch/) by index. |
| [get(string)](#get-string-)| Gets and sets [CellWatch](../cellwatch/) by the name of the cell. |
| [add(number, number)](#add-number-number-)| Adds [Aspose.Cells.CellWatch](../aspose.cells.cellwatch/) with a row and a column. |
| [add(string)](#add-string-)| Adds [Aspose.Cells.CellWatch](../aspose.cells.cellwatch/) with the name of the cell. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets and sets [CellWatch](../cellwatch/) by index.

```javascript
get(index: number) : CellWatch;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[CellWatch](../cellwatch/)

### get(string) {#get-string-}

Gets and sets [CellWatch](../cellwatch/) by the name of the cell.

```javascript
get(cellName: string) : CellWatch;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |

**Returns**

[CellWatch](../cellwatch/)

### add(number, number) {#add-number-number-}

Adds [Aspose.Cells.CellWatch](../aspose.cells.cellwatch/) with a row and a column.

```javascript
add(row: number, column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |

**Returns**

Returns the position of this item in the collection.

### add(string) {#add-string-}

Adds [Aspose.Cells.CellWatch](../aspose.cells.cellwatch/) with the name of the cell.

```javascript
add(cellName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |

### getCount() {#getCount--}

<b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



