---
title: DataModelRelationshipCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the relationships.
type: docs
url: /nodejs-cpp/datamodelrelationshipcollection/
---

## DataModelRelationshipCollection class

Represents the relationships.

```javascript
class DataModelRelationshipCollection implements Iterable<DataModelRelationship>;
```


## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the relationship. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<DataModelRelationship\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### get(number) {#get-number-}

Gets the relationship.

```javascript
get(index: number) : DataModelRelationship;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[DataModelRelationship](../datamodelrelationship/)

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



