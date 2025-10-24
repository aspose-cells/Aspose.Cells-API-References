##CustomGeometry
Represents a custom geometric shape.
## CustomGeometry class
Represents a custom geometric shape.
```javascript
class CustomGeometry extends Geometry;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Geometry)](#constructor-geometry-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [paths](#paths--)| ShapePathCollection | Readonly. Gets path collection information when shape is a NotPrimitive autoshape |
| [shapeAdjustValues](#shapeAdjustValues--)| ShapeGuideCollection | Readonly. Gets a collection of shape adjust value |
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
