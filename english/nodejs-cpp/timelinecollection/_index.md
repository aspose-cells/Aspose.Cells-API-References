﻿---
title: TimelineCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Specifies the collection of all the Timeline objects on the specified worksheet. Due to MS Excel, Excel 2003 does not support Timeline.
type: docs
url: /nodejs-cpp/timelinecollection/
---

## TimelineCollection class

Specifies the collection of all the Timeline objects on the specified worksheet. Due to MS Excel, Excel 2003 does not support Timeline.

```javascript
class TimelineCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the Timeline by index. |
| [add(PivotTable, number, number, string)](#add-pivottable-number-number-string-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, string)](#add-pivottable-string-string-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, number, number, number)](#add-pivottable-number-number-number-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, number)](#add-pivottable-string-number-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, number, number, PivotField)](#add-pivottable-number-number-pivotfield-)| Add a new Timeline using PivotTable as data source |
| [add(PivotTable, string, PivotField)](#add-pivottable-string-pivotfield-)| Add a new Timeline using PivotTable as data source |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets the Timeline by index.

```javascript
get(index: number) : Timeline;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[Timeline](./timeline/)

### add(PivotTable, number, number, string) {#add-pivottable-number-number-string-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### add(PivotTable, string, string) {#add-pivottable-string-string-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, destCellName: string, baseFieldName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseFieldName | string | The name of PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### add(PivotTable, number, number, number) {#add-pivottable-number-number-number-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, row: number, column: number, baseFieldIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### add(PivotTable, string, number) {#add-pivottable-string-number-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, destCellName: string, baseFieldIndex: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseFieldIndex | number | The index of PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### add(PivotTable, number, number, PivotField) {#add-pivottable-number-number-pivotfield-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, row: number, column: number, baseField: PivotField) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| row | number | Row index of the cell in the upper-left corner of the Timeline range. |
| column | number | Column index of the cell in the upper-left corner of the Timeline range. |
| baseField | [PivotField](./pivotfield/) | The PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### add(PivotTable, string, PivotField) {#add-pivottable-string-pivotfield-}

Add a new Timeline using PivotTable as data source

```javascript
add(pivot: PivotTable, destCellName: string, baseField: PivotField) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| pivot | [PivotTable](./pivottable/) | PivotTable object |
| destCellName | string | The cell name in the upper-left corner of the Timeline range. |
| baseField | [PivotField](./pivotfield/) | The PivotField in PivotTable.BaseFields |

**Returns**

The new add Timeline index

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



