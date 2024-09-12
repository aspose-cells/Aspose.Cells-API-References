---
title: ShapeSegmentPathCollection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape.
type: docs
url: /nodejs-cpp/shapesegmentpathcollection/
---

## ShapeSegmentPathCollection class

Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.

```javascript
class ShapeSegmentPathCollection;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |

## Methods

| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets [ShapeSegmentPath](../shapesegmentpath/) object. |
| [add(ShapePathType)](#add-shapepathtype-)| Add a segment path in creation path. |
| [getCount()](#getCount--)| Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |


### constructor() {#constructor--}

Default Constructor.

```javascript
constructor();
```


### get(number) {#get-number-}

Gets [ShapeSegmentPath](../shapesegmentpath/) object.

```javascript
get(index: number) : ShapeSegmentPath;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |

**Returns**

Returns a [ShapeSegmentPath](../shapesegmentpath/) object.

### add(ShapePathType) {#add-shapepathtype-}

Add a segment path in creation path.

```javascript
add(type: ShapePathType) : number;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ShapePathType](../shapepathtype/) | The path type. |

**Returns**

Returns the position of [ShapeSegmentPath](../shapesegmentpath/) object in the list.

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



