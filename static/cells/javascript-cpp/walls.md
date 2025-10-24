##Walls
Encapsulates the object that represents the walls of a 3D chart.
## Walls class
Encapsulates the object that represents the walls of a 3-D chart.
```javascript
class Walls extends Floor;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(Floor)](#constructor-floor-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [centerX](#centerX--)| number | Readonly. Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [centerY](#centerY--)| number | Readonly. Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [width](#width--)| number | Readonly. Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [depth](#depth--)| number | Readonly. Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [height](#height--)| number | Readonly. Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [centerXPx](#centerXPx--)| number | Readonly. Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [centerYPx](#centerYPx--)| number | Readonly. Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [widthPx](#widthPx--)| number | Readonly. Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
| [depthPx](#depthPx--)| number | Readonly. Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [heightPx](#heightPx--)| number | Readonly. Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [formatting](#formatting--)| FormattingType | Represents the formatting of the area. |
| [invertIfNegative](#invertIfNegative--)| boolean | If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [fillFormat](#fillFormat--)| FillFormat | Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [border](#border--)| Line | Gets or sets the border [Line](../line/). |
## Methods
| Method | Description |
| --- | --- |
| [getCubePointCount()](#getCubePointCount--)| Gets the number of cube points after calls Chart.Calculate() method. |
| [getCubePointXPx(number)](#getCubePointXPx-number-)| Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight |
| [getCubePointYPx(number)](#getCubePointYPx-number-)| Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight. |
### constructor(Floor) {#constructor-floor-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: Floor);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Floor | The parent object. |
### centerX {#centerX--}
Readonly. Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```javascript
centerX : number;
```
### centerY {#centerY--}
Readonly. Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```javascript
centerY : number;
```
### width {#width--}
Readonly. Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```javascript
width : number;
```
### depth {#depth--}
Readonly. Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method.
```javascript
depth : number;
```
### height {#height--}
Readonly. Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method.
```javascript
height : number;
```
### centerXPx {#centerXPx--}
Readonly. Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.
```javascript
centerXPx : number;
```
### centerYPx {#centerYPx--}
Readonly. Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method.
```javascript
centerYPx : number;
```
### widthPx {#widthPx--}
Readonly. Gets the width of left to right in units of pixels after calls Chart.Calculate() method.
```javascript
widthPx : number;
```
### depthPx {#depthPx--}
Readonly. Gets the depth front to back in units of pixels after calls Chart.Calculate() method.
```javascript
depthPx : number;
```
### heightPx {#heightPx--}
Readonly. Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method.
```javascript
heightPx : number;
```
### backgroundColor {#backgroundColor--}
Gets or sets the background [Color](../color/) of the [Area](../area/).
```javascript
backgroundColor : Color;
```
### foregroundColor {#foregroundColor--}
Gets or sets the foreground [Color](../color/).
```javascript
foregroundColor : Color;
```
### formatting {#formatting--}
Represents the formatting of the area.
```javascript
formatting : FormattingType;
```
### invertIfNegative {#invertIfNegative--}
If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged.
```javascript
invertIfNegative : boolean;
```
### fillFormat {#fillFormat--}
Readonly. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape.
```javascript
fillFormat : FillFormat;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### border {#border--}
Gets or sets the border [Line](../line/).
```javascript
border : Line;
```
### getCubePointCount() {#getCubePointCount--}
Gets the number of cube points after calls Chart.Calculate() method.
```javascript
getCubePointCount() : number;
```
### getCubePointXPx(number) {#getCubePointXPx-number-}
Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight
```javascript
getCubePointXPx(index: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
### getCubePointYPx(number) {#getCubePointYPx-number-}
Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight.
```javascript
getCubePointYPx(index: number) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number |  |
