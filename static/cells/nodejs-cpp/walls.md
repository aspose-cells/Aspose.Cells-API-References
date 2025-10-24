##Walls
Encapsulates the object that represents the walls of a 3D chart.
## Walls class
Encapsulates the object that represents the walls of a 3-D chart.
```javascript
class Walls extends Floor;
```
## Constructors
| Constructor | Description |
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
| [getCenterX()](#getCenterX--)| <b>@deprecated.</b> Please use the 'centerX' property instead. Gets the x coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getCenterY()](#getCenterY--)| <b>@deprecated.</b> Please use the 'centerY' property instead. Gets the y coordinate of the left-bottom corner of Wall center in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Gets the width of left to right in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getDepth()](#getDepth--)| <b>@deprecated.</b> Please use the 'depth' property instead. Gets the depth front to back in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Gets the height of top to bottom in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [getCenterXPx()](#getCenterXPx--)| <b>@deprecated.</b> Please use the 'centerXPx' property instead. Gets the x coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getCenterYPx()](#getCenterYPx--)| <b>@deprecated.</b> Please use the 'centerYPx' property instead. Gets the y coordinate of the left-bottom corner of Wall center in units of pixels after calls Chart.Calculate() method. |
| [getWidthPx()](#getWidthPx--)| <b>@deprecated.</b> Please use the 'widthPx' property instead. Gets the width of left to right in units of pixels after calls Chart.Calculate() method. |
| [getDepthPx()](#getDepthPx--)| <b>@deprecated.</b> Please use the 'depthPx' property instead. Gets the depth front to back in units of pixels after calls Chart.Calculate() method. |
| [getHeightPx()](#getHeightPx--)| <b>@deprecated.</b> Please use the 'heightPx' property instead. Gets the height of top to bottom in units of pixels after calls Chart.Calculate() method. |
| [getCubePointCount()](#getCubePointCount--)| Gets the number of cube points after calls Chart.Calculate() method. |
| [getCubePointXPx(number)](#getCubePointXPx-number-)| Gets x-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight |
| [getCubePointYPx(number)](#getCubePointYPx-number-)| Gets y-coordinate of the apex point of walls cube after calls Chart.Calculate() method. The number of apex points of walls cube is eight. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [getFormatting()](#getFormatting--)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [setFormatting(FormattingType)](#setFormatting-formattingtype-)| <b>@deprecated.</b> Please use the 'formatting' property instead. Represents the formatting of the area. |
| [getInvertIfNegative()](#getInvertIfNegative--)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [setInvertIfNegative(boolean)](#setInvertIfNegative-boolean-)| <b>@deprecated.</b> Please use the 'invertIfNegative' property instead. If the property is true and the value of chart point is a negative number, the foreground color and background color will be exchanged. |
| [getFillFormat()](#getFillFormat--)| <b>@deprecated.</b> Please use the 'fillFormat' property instead. Represents a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified chart or shape. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getBorder()](#getBorder--)| <b>@deprecated.</b> Please use the 'border' property instead. Gets or sets the border [Line](../line/). |
| [setBorder(Line)](#setBorder-line-)| <b>@deprecated.</b> Please use the 'border' property instead. Gets or sets the border [Line](../line/). |
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
### getCenterX() {#getCenterX--}
```javascript
getCenterX() : number;
```
### getCenterY() {#getCenterY--}
```javascript
getCenterY() : number;
```
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
### getDepth() {#getDepth--}
```javascript
getDepth() : number;
```
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
### getCenterXPx() {#getCenterXPx--}
```javascript
getCenterXPx() : number;
```
### getCenterYPx() {#getCenterYPx--}
```javascript
getCenterYPx() : number;
```
### getWidthPx() {#getWidthPx--}
```javascript
getWidthPx() : number;
```
### getDepthPx() {#getDepthPx--}
```javascript
getDepthPx() : number;
```
### getHeightPx() {#getHeightPx--}
```javascript
getHeightPx() : number;
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
### getBackgroundColor() {#getBackgroundColor--}
```javascript
getBackgroundColor() : Color;
```
**Returns**
[Color](../color/)
### setBackgroundColor(Color) {#setBackgroundColor-color-}
```javascript
setBackgroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getForegroundColor() {#getForegroundColor--}
```javascript
getForegroundColor() : Color;
```
**Returns**
[Color](../color/)
### setForegroundColor(Color) {#setForegroundColor-color-}
```javascript
setForegroundColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getFormatting() {#getFormatting--}
```javascript
getFormatting() : FormattingType;
```
**Returns**
[FormattingType](../formattingtype/)
### setFormatting(FormattingType) {#setFormatting-formattingtype-}
```javascript
setFormatting(value: FormattingType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormattingType](../formattingtype/) | The value to set. |
### getInvertIfNegative() {#getInvertIfNegative--}
```javascript
getInvertIfNegative() : boolean;
```
### setInvertIfNegative(boolean) {#setInvertIfNegative-boolean-}
```javascript
setInvertIfNegative(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getFillFormat() {#getFillFormat--}
```javascript
getFillFormat() : FillFormat;
```
**Returns**
[FillFormat](../fillformat/)
### getTransparency() {#getTransparency--}
```javascript
getTransparency() : number;
```
### setTransparency(number) {#setTransparency-number-}
```javascript
setTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBorder() {#getBorder--}
```javascript
getBorder() : Line;
```
**Returns**
[Line](../line/)
### setBorder(Line) {#setBorder-line-}
```javascript
setBorder(value: Line) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Line](../line/) | The value to set. |
