---
title: ColumnCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Collection of the Columnnodejscppcolumn objects that represent the individual columnsettings in a worksheet. The Column object only represents the settings such as column width styles .etc. for the whole column has nothing to do with the fact that there are nonempty cellsdata or not in corresponding column. And the Count of this collection only represents the count Column objects that have been instantiated in this collection has nothing to do with the fact that there are nonempty cellsdata or not in the worksheet.
type: docs
url: /nodejs-cpp/columncollection/
---

## ColumnCollection class

Collection of the [Column](/nodejs-cpp/column/) objects that represent the individual column(setting)s in a worksheet. The Column object only represents the settings such as column width, styles, .etc. for the whole column, has nothing to do with the fact that there are non-empty cells(data) or not in corresponding column. And the "Count" of this collection only represents the count Column objects that have been instantiated in this collection, has nothing to do with the fact that there are non-empty cells(data) or not in the worksheet.

```javascript
class ColumnCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [Column](/nodejs-cpp/column/) object by column index. The Column object of given column index will be instantiated if it does not exist before. |
| [getColumnByIndex(number)](#getColumnByIndex-number-)| Gets the [Column](/nodejs-cpp/column/) object by the position in the list. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets a [Column](/nodejs-cpp/column/) object by column index. The Column object of given column index will be instantiated if it does not exist before.

```javascript
get(columnIndex: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnIndex | number |  |

**Returns**

[Column](/nodejs-cpp/column/)

### getColumnByIndex(number) {#getColumnByIndex-number-}

Gets the [Column](/nodejs-cpp/column/) object by the position in the list.

```javascript
getColumnByIndex(index: number) : Column;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The position in the list. |

**Returns**

Returns the column object.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



