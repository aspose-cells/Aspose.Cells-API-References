---
title: FilterColumnCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A collection of Filter objects that represents all the filters in an autofiltered range.
type: docs
url: /nodejs-cpp/filtercolumncollection/
---

## FilterColumnCollection class

A collection of Filter objects that represents all the filters in an autofiltered range.

```javascript
class FilterColumnCollection;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [FilterColumn](/nodejs-cpp/filtercolumn/) object at the special field. |
| [removeAt(number)](#removeAt-number-)|  |
| [getByIndex(number)](#getByIndex-number-)| Returns a single Filter object from a collection. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |


### get(number) {#get-number-}

Gets [FilterColumn](/nodejs-cpp/filtercolumn/) object at the special field.

```javascript
get(fieldIndex: number) : FilterColumn;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldIndex | number | The integer offset of the field on which you want to base the filter          /// (from the left of the list; the leftmost field is field 0). |

**Returns**

Returns [FilterColumn](/nodejs-cpp/filtercolumn/) object.

### removeAt(number) {#removeAt-number-}



```javascript
removeAt(index: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

### getByIndex(number) {#getByIndex-number-}

Returns a single Filter object from a collection.

```javascript
getByIndex(index: number) : FilterColumn;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[FilterColumn](/nodejs-cpp/filtercolumn/)

### getCount() {#getCount--}

Gets the number of elements contained in.

```javascript
getCount() : number;
```



