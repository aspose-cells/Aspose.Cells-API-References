##CellsColor
Represents all types of color.
## CellsColor class
Represents all types of color.
```javascript
class CellsColor;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [isShapeColor](#isShapeColor--)| boolean | Gets and set the color which should apply to cell or shape. |
| [type](#type--)| ColorType | Readonly. The color type. |
| [themeColor](#themeColor--)| ThemeColor | Gets the theme color. Only applies for theme color type. |
| [colorIndex](#colorIndex--)| number | Gets and sets the color index in the color palette. Only applies of indexed color. |
| [color](#color--)| Color | Gets and sets the RGB color. |
| [argb](#argb--)| number | Gets and sets the color from a 32-bit ARGB value. |
| [transparency](#transparency--)| number | Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [isShapeColor()](#isShapeColor--)| <b>@deprecated.</b> Please use the 'isShapeColor' property instead. Gets and set the color which should apply to cell or shape. |
| [setIsShapeColor(boolean)](#setIsShapeColor-boolean-)| <b>@deprecated.</b> Please use the 'isShapeColor' property instead. Gets and set the color which should apply to cell or shape. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. The color type. |
| [getThemeColor()](#getThemeColor--)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets the theme color. Only applies for theme color type. |
| [setThemeColor(ThemeColor)](#setThemeColor-themecolor-)| <b>@deprecated.</b> Please use the 'themeColor' property instead. Gets the theme color. Only applies for theme color type. |
| [getColorIndex()](#getColorIndex--)| <b>@deprecated.</b> Please use the 'colorIndex' property instead. Gets and sets the color index in the color palette. Only applies of indexed color. |
| [setColorIndex(number)](#setColorIndex-number-)| <b>@deprecated.</b> Please use the 'colorIndex' property instead. Gets and sets the color index in the color palette. Only applies of indexed color. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the RGB color. |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the RGB color. |
| [getArgb()](#getArgb--)| <b>@deprecated.</b> Please use the 'argb' property instead. Gets and sets the color from a 32-bit ARGB value. |
| [setArgb(number)](#setArgb-number-)| <b>@deprecated.</b> Please use the 'argb' property instead. Gets and sets the color from a 32-bit ARGB value. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTintOfShapeColor(number)](#setTintOfShapeColor-number-)| Set the tint of the shape color |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### isShapeColor {#isShapeColor--}
Gets and set the color which should apply to cell or shape.
```javascript
isShapeColor : boolean;
```
**Remarks**
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
### type {#type--}
Readonly. The color type.
```javascript
type : ColorType;
```
### themeColor {#themeColor--}
Gets the theme color. Only applies for theme color type.
```javascript
themeColor : ThemeColor;
```
### colorIndex {#colorIndex--}
Gets and sets the color index in the color palette. Only applies of indexed color.
```javascript
colorIndex : number;
```
### color {#color--}
Gets and sets the RGB color.
```javascript
color : Color;
```
### argb {#argb--}
Gets and sets the color from a 32-bit ARGB value.
```javascript
argb : number;
```
### transparency {#transparency--}
Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### isShapeColor() {#isShapeColor--}
```javascript
isShapeColor() : boolean;
```
**Remarks**
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
### setIsShapeColor(boolean) {#setIsShapeColor-boolean-}
```javascript
setIsShapeColor(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.
### getType() {#getType--}
```javascript
getType() : ColorType;
```
**Returns**
[ColorType](../colortype/)
### getThemeColor() {#getThemeColor--}
```javascript
getThemeColor() : ThemeColor;
```
**Returns**
[ThemeColor](../themecolor/)
### setThemeColor(ThemeColor) {#setThemeColor-themecolor-}
```javascript
setThemeColor(value: ThemeColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ThemeColor](../themecolor/) | The value to set. |
### getColorIndex() {#getColorIndex--}
```javascript
getColorIndex() : number;
```
### setColorIndex(number) {#setColorIndex-number-}
```javascript
setColorIndex(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getColor() {#getColor--}
```javascript
getColor() : Color;
```
**Returns**
[Color](../color/)
### setColor(Color) {#setColor-color-}
```javascript
setColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getArgb() {#getArgb--}
```javascript
getArgb() : number;
```
### setArgb(number) {#setArgb-number-}
```javascript
setArgb(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
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
### setTintOfShapeColor(number) {#setTintOfShapeColor-number-}
Set the tint of the shape color
```javascript
setTintOfShapeColor(tint: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tint | number |  |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
