---
title: PivotFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a collection of all the PivotFilter objects
type: docs
url: /nodejs-cpp/pivotfiltercollection/
---

## PivotFilterCollection class

Represents a collection of all the PivotFilter objects

```javascript
class PivotFilterCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivotfilter object at the specific index. |
| [add(number, PivotFilterType)](#add-number-pivotfiltertype-)| Adds a PivotFilter Object to the specific type |
| [clearFilter(number)](#clearFilter-number-)| Clear PivotFilter from the specific PivotField |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### get(number) {#get-number-}

Gets the pivotfilter object at the specific index.

```javascript
get(index: number) : PivotFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotFilter](../pivotfilter/)

### add(number, PivotFilterType) {#add-number-pivotfiltertype-}

Adds a PivotFilter Object to the specific type

```javascript
add(fieldIndex: number, type: PivotFilterType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | the PivotField index |
| type | [PivotFilterType](../pivotfiltertype/) | the PivotFilter type |

**Returns**

the index of  the PivotFilter Object in this PivotFilterCollection.

### clearFilter(number) {#clearFilter-number-}

Clear PivotFilter from the specific PivotField

```javascript
clearFilter(fieldIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | the PivotField index |

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```


### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```



