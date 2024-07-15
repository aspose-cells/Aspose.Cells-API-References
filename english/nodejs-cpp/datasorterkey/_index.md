---
title: DataSorterKey
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the key of the data sorter.
type: docs
url: /nodejs-cpp/datasorterkey/
---

## DataSorterKey class

Represents the key of the data sorter.

```javascript
class DataSorterKey;
```


## Methods

| Method | Description |
| --- | --- |
| [getOrder()](#getOrder--)| Indicates the order of sorting. |
| [getIndex()](#getIndex--)| Gets the sorted column index(absolute position, column A is 0, B is 1, ...). |
| [getType()](#getType--)| Represents the type of sorting. |
| [getIconSetType()](#getIconSetType--)| Represents the icon set type. |
| [getIconId()](#getIconId--)| Represents the id of the icon set type. |
| [getColor()](#getColor--)| Gets the sorted color. |


### getOrder() {#getOrder--}

Indicates the order of sorting.

```javascript
getOrder() : SortOrder;
```


**Returns**

[SortOrder](../sortorder/)

### getIndex() {#getIndex--}

Gets the sorted column index(absolute position, column A is 0, B is 1, ...).

```javascript
getIndex() : number;
```


### getType() {#getType--}

Represents the type of sorting.

```javascript
getType() : SortOnType;
```


**Returns**

[SortOnType](../sortontype/)

### getIconSetType() {#getIconSetType--}

Represents the icon set type.

```javascript
getIconSetType() : IconSetType;
```


**Returns**

[IconSetType](../iconsettype/)

**Remarks**

Only takes effect when [Type](../type/) is [Type](../type/).

### getIconId() {#getIconId--}

Represents the id of the icon set type.

```javascript
getIconId() : number;
```


**Remarks**

Only takes effect when [Type](../type/) is [Type](../type/).

### getColor() {#getColor--}

Gets the sorted color.

```javascript
getColor() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

Only takes effect when [Type](../type/) is [Type](../type/) or [Type](../type/).


