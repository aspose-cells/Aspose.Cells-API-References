﻿---
title: TableStyleElementCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents all elements of the table style.
type: docs
url: /javascript-cpp/tablestyleelementcollection/
---

## TableStyleElementCollection class

Represents all elements of the table style.

```javascript
class TableStyleElementCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets an element of the table style by the index. |
| [get(TableStyleElementType)](#get-tablestyleelementtype-)| Gets the element of the table style by the element type. |
| [add(TableStyleElementType)](#add-tablestyleelementtype-)| Adds an element. |


### get(number) {#get-number-}

Gets an element of the table style by the index.

```javascript
get(index: number) : TableStyleElement;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

Returns [TableStyleElement](../tablestyleelement/) object

### get(TableStyleElementType) {#get-tablestyleelementtype-}

Gets the element of the table style by the element type.

```javascript
get(type: TableStyleElementType) : TableStyleElement;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TableStyleElementType](../tablestyleelementtype/) | The element type. |

**Returns**

Returns [TableStyleElement](../tablestyleelement/) object

### add(TableStyleElementType) {#add-tablestyleelementtype-}

Adds an element.

```javascript
add(type: TableStyleElementType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [TableStyleElementType](../tablestyleelementtype/) | The type of the element |

**Returns**

Returns the index of the element in the list.


