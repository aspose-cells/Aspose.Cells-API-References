##ShapePathPoint
Specify position coordinates or angle markers. Position coordinates represent the coordinates of a path in a coordinate space e.g. XY. Angle markers indicate angular changes in a path e.g. the start and swing angles of an arc.
## ShapePathPoint class
Specify position coordinates or angle markers. Position coordinates represent the coordinates of a path in a coordinate space (e.g. X/Y). Angle markers indicate angular changes in a path (e.g. the start and swing angles of an arc).
```javascript
class ShapePathPoint;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [x](#x--)| number | Gets and sets x coordinate for this position coordinate. Unit EMUs. |
| [y](#y--)| number | Gets y coordinate for this position coordinate. Unit EMUs. |
| [xPixel](#xPixel--)| number | When the object is a position coordinate, get or set the x coordinate in pixels. |
| [yPixel](#yPixel--)| number | When the object is a position coordinate, get or set the y coordinate in pixels. |
| [xAngle](#xAngle--)| number | When the object is an angle marker, get or set the first angle in degrees. |
| [yAngle](#yAngle--)| number | When the object is an angle marker, get or set the second angle in degrees. |
| [type](#type--)| ShapePathPointValueType | Readonly. Specifies the value type of the current object. |
### x {#x--}
Gets and sets x coordinate for this position coordinate. Unit EMUs.
```javascript
x : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### y {#y--}
Gets y coordinate for this position coordinate. Unit EMUs.
```javascript
y : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### xPixel {#xPixel--}
When the object is a position coordinate, get or set the x coordinate in pixels.
```javascript
xPixel : number;
```
### yPixel {#yPixel--}
When the object is a position coordinate, get or set the y coordinate in pixels.
```javascript
yPixel : number;
```
### xAngle {#xAngle--}
When the object is an angle marker, get or set the first angle in degrees.
```javascript
xAngle : number;
```
**Remarks**
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
### yAngle {#yAngle--}
When the object is an angle marker, get or set the second angle in degrees.
```javascript
yAngle : number;
```
**Remarks**
If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.
### type {#type--}
Readonly. Specifies the value type of the current object.
```javascript
type : ShapePathPointValueType;
```
