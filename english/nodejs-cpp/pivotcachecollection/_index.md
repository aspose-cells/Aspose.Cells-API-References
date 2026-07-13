---
title: PivotCacheCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the collection of memory caches from the PivotTable reports in a workbook.
type: docs
url: /nodejs-cpp/pivotcachecollection/
---

## PivotCacheCollection class

Represents the collection of memory caches from the PivotTable reports in a workbook.

```javascript
class PivotCacheCollection implements Iterable<PivotCache>;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the pivot table cache at the specified index. |
| [dispose()](#dispose--)| Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<PivotCache\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets the pivot table cache at the specified index.

```javascript
get(index: number) : PivotCache;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[PivotCache](../pivotcache/)

### dispose() {#dispose--}

Performs application-defined tasks associated with freeing, releasing, or resetting unmanaged resources.

```javascript
dispose() : void;
```


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



