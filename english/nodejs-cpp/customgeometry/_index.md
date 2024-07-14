---
title: CustomGeometry
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents a custom geometric shape.
type: docs
url: /nodejs-cpp/customgeometry/
---

## CustomGeometry class

Represents a custom geometric shape.

```javascript
class CustomGeometry extends Geometry;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Geometry)](#constructor-geometry-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getPaths()](#getPaths--)| Gets path collection information when shape is a NotPrimitive autoshape |
| [getShapeAdjustValues()](#getShapeAdjustValues--)| Gets a collection of shape adjust value |


### constructor(Geometry) {#constructor-geometry-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Geometry);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Geometry | The parent object. |

### getPaths() {#getPaths--}

Gets path collection information when shape is a NotPrimitive autoshape

```javascript
getPaths() : ShapePathCollection;
```


**Returns**

[ShapePathCollection](/nodejs-cpp/shapepathcollection/)

### getShapeAdjustValues() {#getShapeAdjustValues--}

Gets a collection of shape adjust value

```javascript
getShapeAdjustValues() : ShapeGuideCollection;
```


**Returns**

[ShapeGuideCollection](/nodejs-cpp/shapeguidecollection/)


