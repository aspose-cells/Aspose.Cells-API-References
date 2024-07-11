---
title: PivotItemCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection of all the PivotItem objects in the PivotField's
type: docs
url: /nodejs-cpp/pivotitemcollection/
---

## PivotItemCollection class

Represents a collection of all the PivotItem objects in the PivotField's

```javascript
class PivotItemCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotItem Object at the specific index. |
| [getCount()](#getCount--)| Gets the count of the pivot items. |
| [getEnumerator()](#getEnumerator--)| Gets an enumerator over the elements in this collection in proper sequence. |
| [changeitemsOrder(number, number)](#changeitemsOrder-number-number-)| Directly changes the orders of the two items. |


### get(number) {#get-number-}

Gets the PivotItem Object at the specific index.

```javascript
get(index: number) : PivotItem;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotItem](./pivotitem/)

### getCount() {#getCount--}

Gets the count of the pivot items.

```javascript
getCount() : number;
```


### getEnumerator() {#getEnumerator--}

Gets an enumerator over the elements in this collection in proper sequence.

```javascript
getEnumerator() : PivotItemEnumerator;
```


**Returns**

enumerator

### changeitemsOrder(number, number) {#changeitemsOrder-number-number-}

Directly changes the orders of the two items.

```javascript
changeitemsOrder(sourceIndex: number, destIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | number | The current index |
| destIndex | number | The dest index |


