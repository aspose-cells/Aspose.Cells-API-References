##CustomGeometry
Represents a custom geometric shape.
## CustomGeometry class
Represents a custom geometric shape.
```javascript
class CustomGeometry extends Geometry;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(Geometry)](#constructor-geometry-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [paths](#paths--)| ShapePathCollection | Readonly. Gets path collection information when shape is a NotPrimitive autoshape |
| [shapeAdjustValues](#shapeAdjustValues--)| ShapeGuideCollection | Readonly. Gets a collection of shape adjust value |
## Methods
| Method | Description |
| --- | --- |
| [getPaths()](#getPaths--)| <b>@deprecated.</b> Please use the 'paths' property instead. Gets path collection information when shape is a NotPrimitive autoshape |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getShapeAdjustValues()](#getShapeAdjustValues--)| <b>@deprecated.</b> Please use the 'shapeAdjustValues' property instead. Gets a collection of shape adjust value |
### constructor(Geometry) {#constructor-geometry-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Geometry);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Geometry | The parent object. |
### paths {#paths--}
Readonly. Gets path collection information when shape is a NotPrimitive autoshape
```javascript
paths : ShapePathCollection;
```
### shapeAdjustValues {#shapeAdjustValues--}
Readonly. Gets a collection of shape adjust value
```javascript
shapeAdjustValues : ShapeGuideCollection;
```
### getPaths() {#getPaths--}
```javascript
getPaths() : ShapePathCollection;
```
**Returns**
[ShapePathCollection](../shapepathcollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getShapeAdjustValues() {#getShapeAdjustValues--}
```javascript
getShapeAdjustValues() : ShapeGuideCollection;
```
**Returns**
[ShapeGuideCollection](../shapeguidecollection/)
