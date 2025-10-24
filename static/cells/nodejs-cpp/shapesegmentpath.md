##ShapeSegmentPath
Represents a segment path in a path of the freeform.
## ShapeSegmentPath class
Represents a segment path in a path of the freeform.
```javascript
class ShapeSegmentPath;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [type](#type--)| ShapePathType | Readonly. Gets the path segment type |
| [points](#points--)| ShapePathPointCollection | Readonly. Gets the points in path segment |
## Methods
| Method | Description |
| --- | --- |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets the path segment type |
| [getPoints()](#getPoints--)| <b>@deprecated.</b> Please use the 'points' property instead. Gets the points in path segment |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### type {#type--}
Readonly. Gets the path segment type
```javascript
type : ShapePathType;
```
### points {#points--}
Readonly. Gets the points in path segment
```javascript
points : ShapePathPointCollection;
```
### getType() {#getType--}
```javascript
getType() : ShapePathType;
```
**Returns**
[ShapePathType](../shapepathtype/)
### getPoints() {#getPoints--}
```javascript
getPoints() : ShapePathPointCollection;
```
**Returns**
[ShapePathPointCollection](../shapepathpointcollection/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
