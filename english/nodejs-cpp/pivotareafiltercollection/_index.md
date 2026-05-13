---
title: PivotAreaFilterCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the list of filters for PivotArea..pivotarea
type: docs
url: /nodejs-cpp/pivotareafiltercollection/
---

## PivotAreaFilterCollection class

Represents the list of filters for [PivotArea](../pivotarea/)

```javascript
class PivotAreaFilterCollection implements Iterable<PivotAreaFilter>;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets filter from the list by the index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<PivotAreaFilter\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets filter from the list by the index.

```javascript
get(index: number) : PivotAreaFilter;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The Index |

**Returns**

[PivotAreaFilter](../pivotareafilter/)

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



