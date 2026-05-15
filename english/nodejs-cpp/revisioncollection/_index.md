---
title: RevisionCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all revision logs.
type: docs
url: /nodejs-cpp/revisioncollection/
---

## RevisionCollection class

Represents all revision logs.

```javascript
class RevisionCollection implements Iterable<Revision>;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [Revision](../revision/) by the index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<Revision\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets [Revision](../revision/) by the index.

```javascript
get(index: number) : Revision;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |

**Returns**

[Revision](../revision/)

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



