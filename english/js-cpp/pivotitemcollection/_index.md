﻿---
title: PivotItemCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents all the PivotItem..pivotitem objects in the PivotField.
type: docs
url: /js-cpp/pivotitemcollection/
---

## PivotItemCollection class

Represents all the [PivotItem](../pivotitem/) objects in the PivotField.

```javascript
class PivotItemCollection;
```


## Properties

| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the pivot items. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotItem Object at the specific index. |
| [get(string)](#get-string-)| Gets the [PivotItem](../pivotitem/) by the specific name. |
| [getEnumerator()](#getEnumerator--)| Gets an enumerator over the elements in this collection in proper sequence. |
| [swapItem(number, number)](#swapItem-number-number-)| Directly swap two items. |


### count {#count--}

Readonly. Gets the count of the pivot items.

```javascript
count : number;
```


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

[PivotItem](../pivotitem/)

### get(string) {#get-string-}

Gets the [PivotItem](../pivotitem/) by the specific name.

```javascript
get(itemValue: string) : PivotItem;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| itemValue | string |  |

**Returns**

[PivotItem](../pivotitem/)

### getEnumerator() {#getEnumerator--}

Gets an enumerator over the elements in this collection in proper sequence.

```javascript
getEnumerator() : PivotItemEnumerator;
```


**Returns**

enumerator

### swapItem(number, number) {#swapItem-number-number-}

Directly swap two items.

```javascript
swapItem(index1: number, index2: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index1 | number |  |
| index2 | number |  |


