##ShapePath
Represents a creation path consisting of a series of moves lines and curves that when combined will form a geometric shape.
## ShapePath class
Represents a creation path consisting of a series of moves, lines and curves that when combined will form a geometric shape.
```javascript
class ShapePath;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor()](#constructor--)| Initializes a new instance of the [ShapePath](../shapepath/) class. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pathSegementList](#pathSegementList--)| ShapeSegmentPathCollection | Readonly. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list |
| [widthPixel](#widthPixel--)| number | Gets the width of this path in unit of pixels. |
| [heightPixel](#heightPixel--)| number | Gets the height of this path in unit of pixels. |
## Methods
| Method | Description |
| --- | --- |
| [getPathSegementList()](#getPathSegementList--)| <b>@deprecated.</b> Please use the 'pathSegementList' property instead. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list |
| [getWidthPixel()](#getWidthPixel--)| <b>@deprecated.</b> Please use the 'widthPixel' property instead. Gets the width of this path in unit of pixels. |
| [setWidthPixel(number)](#setWidthPixel-number-)| <b>@deprecated.</b> Please use the 'widthPixel' property instead. Gets the width of this path in unit of pixels. |
| [getHeightPixel()](#getHeightPixel--)| <b>@deprecated.</b> Please use the 'heightPixel' property instead. Gets the height of this path in unit of pixels. |
| [setHeightPixel(number)](#setHeightPixel-number-)| <b>@deprecated.</b> Please use the 'heightPixel' property instead. Gets the height of this path in unit of pixels. |
| [moveTo(number, number)](#moveTo-number-number-)| Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel. |
| [lineTo(number, number)](#lineTo-number-number-)| Appends a line segment to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [cubicBezierTo(number, number, number, number, number, number)](#cubicBezierTo-number-number-number-number-number-number-)| Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel. |
| [arcTo(number, number, number, number)](#arcTo-number-number-number-number-)| Appends an elliptical arc to the current figure. The starting point is the end point of the current figure. |
| [close()](#close--)| Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor() {#constructor--}
Initializes a new instance of the [ShapePath](../shapepath/) class.
```javascript
constructor();
```
### pathSegementList {#pathSegementList--}
Readonly. Gets [ShapeSegmentPathCollection](../shapesegmentpathcollection/) list
```javascript
pathSegementList : ShapeSegmentPathCollection;
```
### widthPixel {#widthPixel--}
Gets the width of this path in unit of pixels.
```javascript
widthPixel : number;
```
### heightPixel {#heightPixel--}
Gets the height of this path in unit of pixels.
```javascript
heightPixel : number;
```
### getPathSegementList() {#getPathSegementList--}
```javascript
getPathSegementList() : ShapeSegmentPathCollection;
```
**Returns**
[ShapeSegmentPathCollection](../shapesegmentpathcollection/)
### getWidthPixel() {#getWidthPixel--}
```javascript
getWidthPixel() : number;
```
### setWidthPixel(number) {#setWidthPixel-number-}
```javascript
setWidthPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeightPixel() {#getHeightPixel--}
```javascript
getHeightPixel() : number;
```
### setHeightPixel(number) {#setHeightPixel-number-}
```javascript
setHeightPixel(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### moveTo(number, number) {#moveTo-number-number-}
Starts a new figure from the specified point without closing the current figure. All subsequent points added to the path are added to this new figure.Unit: Pixel.
```javascript
moveTo(x: number, y: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | number | The x-coordinate of the starting point of the figure(Unit: Pixel). |
| y | number | The y-coordinate of the starting point of the figure(Unit: Pixel). |
### lineTo(number, number) {#lineTo-number-number-}
Appends a line segment to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
```javascript
lineTo(x: number, y: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| x | number | The x-coordinate of the endpoint of the line segment(Unit: Pixel). |
| y | number | The y-coordinate of the endpoint of the line segment(Unit: Pixel). |
### cubicBezierTo(number, number, number, number, number, number) {#cubicBezierTo-number-number-number-number-number-number-}
Appends a cubic Bézier curve to the current figure. The starting point is the end point of the current figure.Unit: Pixel.
```javascript
cubicBezierTo(ctrX1: number, ctrY1: number, ctrX2: number, ctrY2: number, endX: number, endY: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ctrX1 | number | The x-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrY1 | number | The y-coordinate of the first control point for the curve(Unit: Pixel). |
| ctrX2 | number | The x-coordinate of the second control point for the curve(Unit: Pixel). |
| ctrY2 | number | The y-coordinate of the second control point for the curve(Unit: Pixel). |
| endX | number | The x-coordinate of the endpoint of the curve(Unit: Pixel). |
| endY | number | The y-coordinate of the endpoint of the curve(Unit: Pixel). |
### arcTo(number, number, number, number) {#arcTo-number-number-number-number-}
Appends an elliptical arc to the current figure. The starting point is the end point of the current figure.
```javascript
arcTo(wR: number, hR: number, stAng: number, swAng: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| wR | number | The half-width of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| hR | number | The half-height of the rectangular area of ​​the ellipse that draws the arc(Unit: Pixel). |
| stAng | number | The starting angle of the arc, measured in degrees clockwise from the x-axis(Unit: Degree). This angle will specify what angle along the supposed circle path will be used as the start position for drawing the arc. This start angle will be locked to the last known pen position in the shape path. Thus guaranteeing a continuos shape path. |
| swAng | number | The swing angle for an arc. This angle will specify how far angle-wise along the supposed cicle path the arc will be extended. The extension from the start angle will always be in the clockwise direction around the supposed circle.(Unit: Degree) |
### close() {#close--}
Closes the current figure and starts a new figure. If the current figure contains a sequence of connected lines and curves, the method closes the loop by connecting a line from the endpoint to the starting point.
```javascript
close() : void;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
