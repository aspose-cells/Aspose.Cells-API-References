---
title: PivotItemCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all the PivotItem..pivotitem objects in the PivotField.
type: docs
url: /nodejs-cpp/pivotitemcollection/
---

## PivotItemCollection class

Represents all the [PivotItem](../pivotitem/) objects in the PivotField.

```javascript
class PivotItemCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotItem Object at the specific index. |
| [get(string)](#get-string-)| Gets the [PivotItem](../pivotitem/) by the specific name. |
| [getCount()](#getCount--)| Gets the count of the pivot items. |
| [getEnumerator()](#getEnumerator--)| Gets an enumerator over the elements in this collection in proper sequence. |
| [swapItem(number, number)](#swapItem-number-number-)| Directly swap two items. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


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

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



