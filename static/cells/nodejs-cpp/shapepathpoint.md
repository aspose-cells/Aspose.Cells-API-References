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
## Methods
| Method | Description |
| --- | --- |
| [getX()](#getX--)| <b>@deprecated.</b> Please use the 'x' property instead. Gets and sets x coordinate for this position coordinate. Unit EMUs. |
| [setX(number)](#setX-number-)| <b>@deprecated.</b> Please use the 'x' property instead. Gets and sets x coordinate for this position coordinate. Unit EMUs. |
| [getY()](#getY--)| <b>@deprecated.</b> Please use the 'y' property instead. Gets y coordinate for this position coordinate. Unit EMUs. |
| [setY(number)](#setY-number-)| <b>@deprecated.</b> Please use the 'y' property instead. Gets y coordinate for this position coordinate. Unit EMUs. |
| [getXPixel()](#getXPixel--)| <b>@deprecated.</b> Please use the 'xPixel' property instead. When the object is a position coordinate, get or set the x coordinate in pixels. |
| [setXPixel(number)](#setXPixel-number-)| <b>@deprecated.</b> Please use the 'xPixel' property instead. When the object is a position coordinate, get or set the x coordinate in pixels. |
| [getYPixel()](#getYPixel--)| <b>@deprecated.</b> Please use the 'yPixel' property instead. When the object is a position coordinate, get or set the y coordinate in pixels. |
| [setYPixel(number)](#setYPixel-number-)| <b>@deprecated.</b> Please use the 'yPixel' property instead. When the object is a position coordinate, get or set the y coordinate in pixels. |
| [getXAngle()](#getXAngle--)| <b>@deprecated.</b> Please use the 'xAngle' property instead. When the object is an angle marker, get or set the first angle in degrees. |
| [setXAngle(number)](#setXAngle-number-)| <b>@deprecated.</b> Please use the 'xAngle' property instead. When the object is an angle marker, get or set the first angle in degrees. |
| [getYAngle()](#getYAngle--)| <b>@deprecated.</b> Please use the 'yAngle' property instead. When the object is an angle marker, get or set the second angle in degrees. |
| [setYAngle(number)](#setYAngle-number-)| <b>@deprecated.</b> Please use the 'yAngle' property instead. When the object is an angle marker, get or set the second angle in degrees. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Specifies the value type of the current object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getX() {#getX--}
```javascript
getX() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### setX(number) {#setX-number-}
```javascript
setX(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.XPixel and ShapePathPoint.XAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### getY() {#getY--}
```javascript
getY() : number;
```
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### setY(number) {#setY-number-}
```javascript
setY(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
NOTE: This member is now obsolete. Instead, please use ShapePathPoint.YPixel and ShapePathPoint.YAngle properties. This property will be removed 12 months later since August 2025. Aspose apologizes for any inconvenience you may have experienced.
### getXPixel() {#getXPixel--}
```javascript
getXPixel() : number;
```
### setXPixel(number) {#setXPixel-number-}
```javascript
setXPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getYPixel() {#getYPixel--}
```javascript
getYPixel() : number;
```
### setYPixel(number) {#setYPixel-number-}
```javascript
setYPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getXAngle() {#getXAngle--}
```javascript
getXAngle() : number;
```
**Remarks**
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
### setXAngle(number) {#setXAngle-number-}
```javascript
setXAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
If this angle is the starting angle of an arc. This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path.
### getYAngle() {#getYAngle--}
```javascript
getYAngle() : number;
```
**Remarks**
If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.
### setYAngle(number) {#setYAngle-number-}
```javascript
setYAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
**Remarks**
If this angle is the swing angle of an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.
### getType() {#getType--}
```javascript
getType() : ShapePathPointValueType;
```
**Returns**
[ShapePathPointValueType](../shapepathpointvaluetype/)
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
