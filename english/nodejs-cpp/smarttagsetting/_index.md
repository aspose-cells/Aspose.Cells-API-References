---
title: SmartTagSetting
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all SmartTagCollection..smarttagcollection object in the worksheet.
type: docs
url: /nodejs-cpp/smarttagsetting/
---

## SmartTagSetting class

Represents all [SmartTagCollection](../smarttagcollection/) object in the worksheet.

```javascript
class SmartTagSetting;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTagCollection](../smarttagcollection/) object by the index. |
| [add(number, number)](#add-number-number-)| Adds a [SmartTagCollection](../smarttagcollection/) object to a cell. |
| [add(string)](#add-string-)| Add a cell smart tags. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets a [SmartTagCollection](../smarttagcollection/) object by the index.

```javascript
get(index: number) : SmartTagCollection;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the [SmartTagCollection](../smarttagcollection/) object in the list. |

**Returns**

[SmartTagCollection](../smarttagcollection/)

### add(number, number) {#add-number-number-}

Adds a [SmartTagCollection](../smarttagcollection/) object to a cell.

```javascript
add(row: number, column: number) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row of the cell. |
| column | number | The column of the cell. |

**Returns**

Returns index of a [SmartTagCollection](../smarttagcollection/) object in the worksheet.

### add(string) {#add-string-}

Add a cell smart tags.

```javascript
add(cellName: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellName | string | The name of the cell. |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



