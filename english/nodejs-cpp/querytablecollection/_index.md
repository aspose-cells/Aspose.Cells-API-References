---
title: QueryTableCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: A collection of QueryTableCollection..querytablecollection objects that represent QueryTable collection information.
type: docs
url: /nodejs-cpp/querytablecollection/
---

## QueryTableCollection class

A collection of [QueryTableCollection](../querytablecollection/) objects that represent QueryTable collection information.

```javascript
class QueryTableCollection implements Iterable<QueryTable>;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the querytable by the specific index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<QueryTable\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets the querytable by the specific index.

```javascript
get(index: number) : QueryTable;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

The querytable

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



