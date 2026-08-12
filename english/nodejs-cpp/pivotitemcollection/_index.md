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
class PivotItemCollection implements Iterable<PivotItem>;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the PivotItem Object at the specific index. |
| [get(string)](#get-string-)| Gets the [PivotItem](../pivotitem/) by the specific name. |
| [hideAllDetail(boolean)](#hideAllDetail-boolean-)| Sets whether to hide all detail of all PivotItems in a pivot field. That is collapse/expand this field. |
| [swapItem(number, number)](#swapItem-number-number-)| Directly swap two items. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<PivotItem\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



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

### hideAllDetail(boolean) {#hideAllDetail-boolean-}

Sets whether to hide all detail of all PivotItems in a pivot field. That is collapse/expand this field.

```javascript
hideAllDetail(isHiddenDetail: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isHiddenDetail | boolean | Whether hide the detail of the pivot field. |

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



