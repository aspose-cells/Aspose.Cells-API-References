##PatternFill
Encapsulates the object that represents pattern fill format
## PatternFill class
Encapsulates the object that represents pattern fill format
```javascript
class PatternFill;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pattern](#pattern--)| FillPattern | Gets or sets the fill pattern type |
| [backgroundColor](#backgroundColor--)| Color | Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [backgroundCellsColor](#backgroundCellsColor--)| CellsColor | Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [foregroundColor](#foregroundColor--)| Color | Gets or sets the foreground [Color](../color/). |
| [foregroundCellsColor](#foregroundCellsColor--)| CellsColor | Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [foreTransparency](#foreTransparency--)| number | Gets or sets the transparency of foreground color. |
| [backTransparency](#backTransparency--)| number | Gets or sets the transparency of background color. |
## Methods
| Method | Description |
| --- | --- |
| [getPattern()](#getPattern--)| <b>@deprecated.</b> Please use the 'pattern' property instead. Gets or sets the fill pattern type |
| [setPattern(FillPattern)](#setPattern-fillpattern-)| <b>@deprecated.</b> Please use the 'pattern' property instead. Gets or sets the fill pattern type |
| [getBackgroundColor()](#getBackgroundColor--)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [setBackgroundColor(Color)](#setBackgroundColor-color-)| <b>@deprecated.</b> Please use the 'backgroundColor' property instead. Gets or sets the background [Color](../color/) of the [Area](../area/). |
| [getBackgroundCellsColor()](#getBackgroundCellsColor--)| <b>@deprecated.</b> Please use the 'backgroundCellsColor' property instead. Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [setBackgroundCellsColor(CellsColor)](#setBackgroundCellsColor-cellscolor-)| <b>@deprecated.</b> Please use the 'backgroundCellsColor' property instead. Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [getForegroundColor()](#getForegroundColor--)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [setForegroundColor(Color)](#setForegroundColor-color-)| <b>@deprecated.</b> Please use the 'foregroundColor' property instead. Gets or sets the foreground [Color](../color/). |
| [getForegroundCellsColor()](#getForegroundCellsColor--)| <b>@deprecated.</b> Please use the 'foregroundCellsColor' property instead. Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [setForegroundCellsColor(CellsColor)](#setForegroundCellsColor-cellscolor-)| <b>@deprecated.</b> Please use the 'foregroundCellsColor' property instead. Gets and sets the foreground [CellsColor](../cellscolor/) object. |
| [getForeTransparency()](#getForeTransparency--)| <b>@deprecated.</b> Please use the 'foreTransparency' property instead. Gets or sets the transparency of foreground color. |
| [setForeTransparency(number)](#setForeTransparency-number-)| <b>@deprecated.</b> Please use the 'foreTransparency' property instead. Gets or sets the transparency of foreground color. |
| [getBackTransparency()](#getBackTransparency--)| <b>@deprecated.</b> Please use the 'backTransparency' property instead. Gets or sets the transparency of background color. |
| [setBackTransparency(number)](#setBackTransparency-number-)| <b>@deprecated.</b> Please use the 'backTransparency' property instead. Gets or sets the transparency of background color. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### pattern {#pattern--}
Gets or sets the fill pattern type
```javascript
pattern : FillPattern;
```
### backgroundColor {#backgroundColor--}
Gets or sets the background [Color](../color/) of the [Area](../area/).
```javascript
backgroundColor : Color;
```
### backgroundCellsColor {#backgroundCellsColor--}
Gets and sets the foreground [CellsColor](../cellscolor/) object.
```javascript
backgroundCellsColor : CellsColor;
```
### foregroundColor {#foregroundColor--}
Gets or sets the foreground [Color](../color/).
```javascript
foregroundColor : Color;
```
### foregroundCellsColor {#foregroundCellsColor--}
Gets and sets the foreground [CellsColor](../cellscolor/) object.
```javascript
foregroundCellsColor : CellsColor;
```
### foreTransparency {#foreTransparency--}
Gets or sets the transparency of foreground color.
```javascript
foreTransparency : number;
```
### backTransparency {#backTransparency--}
Gets or sets the transparency of background color.
```javascript
backTransparency : number;
```
### getPattern() {#getPattern--}
```javascript
getPattern() : FillPattern;
```
**Returns**
[FillPattern](../fillpattern/)
### setPattern(FillPattern) {#setPattern-fillpattern-}
```javascript
setPattern(value: FillPattern) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillPattern](../fillpattern/) | The value to set. |
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
### getBackgroundCellsColor() {#getBackgroundCellsColor--}
```javascript
getBackgroundCellsColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setBackgroundCellsColor(CellsColor) {#setBackgroundCellsColor-cellscolor-}
```javascript
setBackgroundCellsColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
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
### getForegroundCellsColor() {#getForegroundCellsColor--}
```javascript
getForegroundCellsColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setForegroundCellsColor(CellsColor) {#setForegroundCellsColor-cellscolor-}
```javascript
setForegroundCellsColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
### getForeTransparency() {#getForeTransparency--}
```javascript
getForeTransparency() : number;
```
### setForeTransparency(number) {#setForeTransparency-number-}
```javascript
setForeTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getBackTransparency() {#getBackTransparency--}
```javascript
getBackTransparency() : number;
```
### setBackTransparency(number) {#setBackTransparency-number-}
```javascript
setBackTransparency(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
