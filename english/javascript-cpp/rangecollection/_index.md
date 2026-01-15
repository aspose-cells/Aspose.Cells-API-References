---
title: RangeCollection
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Encapsulates a collection of Range..range objects.
type: docs
url: /javascript-cpp/rangecollection/
---

## RangeCollection class

Encapsulates a collection of [Range](../range/) objects.

```javascript
class RangeCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the [Range](../range/) element at the specified index. |
| [add(Range)](#add-range-)| Adds a [Range](../range/) item to the collection. |
| [addRange(Range)](#addRange-range-)| Adds a [Range](../range/) item to the collection. |


### get(number) {#get-number-}

Gets the [Range](../range/) element at the specified index.

```javascript
get(index: number) : Range;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The zero based index of the element. |

**Returns**

The element at the specified index.

### add(Range) {#add-range-}

Adds a [Range](../range/) item to the collection.

```javascript
add(range: Range) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | Range object |

**Remarks**

NOTE: This member is now obsolete. Instead, please use AddRange() method. This method will be removed 6 months later since December 2025. Aspose apologizes for any inconvenience you may have experienced.

### addRange(Range) {#addRange-range-}

Adds a [Range](../range/) item to the collection.

```javascript
addRange(range: Range) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| range | [Range](../range/) | the range to be added |

**Returns**

index of the added range in this collection


