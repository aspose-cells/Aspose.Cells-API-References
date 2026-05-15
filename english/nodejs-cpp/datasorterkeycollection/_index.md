---
title: DataSorterKeyCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the key list of data sorter.
type: docs
url: /nodejs-cpp/datasorterkeycollection/
---

## DataSorterKeyCollection class

Represents the key list of data sorter.

```javascript
class DataSorterKeyCollection implements Iterable<DataSorterKey>;
```


## Constructors

| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets and sets [DataSorterKey](../datasorterkey/) by index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |

## \[Symbol.iterator\](): Iterator\<DataSorterKey\>

Returns an iterator over the items in the collection. Enables use of `for...of`, spread syntax, and `Array.from()`.



### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets and sets [DataSorterKey](../datasorterkey/) by index.

```javascript
get(index: number) : DataSorterKey;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

[DataSorterKey](../datasorterkey/)

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



