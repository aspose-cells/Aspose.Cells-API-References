---
title: SmartTagCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all smart tags in the cell.
type: docs
url: /nodejs-cpp/smarttagcollection/
---

## SmartTagCollection class

Represents all smart tags in the cell.

```javascript
class SmartTagCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets a [SmartTag](./smarttag/) object at the specific index |
| [getRow()](#getRow--)| Gets the row of the cell smart tags. |
| [getColumn()](#getColumn--)| Gets the column of the cell smart tags. |
| [add(string, string)](#add-string-string-)| Adds a smart tag. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets a [SmartTag](./smarttag/) object at the specific index

```javascript
get(index: number) : SmartTag;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

returns a [SmartTag](./smarttag/) object.

### getRow() {#getRow--}

Gets the row of the cell smart tags.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets the column of the cell smart tags.

```javascript
getColumn() : number;
```


### add(string, string) {#add-string-string-}

Adds a smart tag.

```javascript
add(uri: string, name: string) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| uri | string | Specifies the namespace URI of the smart tag |
| name | string | Specifies the name of the smart tag. |

**Returns**

The index of smart tag in the list.

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



