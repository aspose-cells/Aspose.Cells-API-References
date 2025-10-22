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
| [setTintOfShapeColor(number)](#setTintOfShapeColor-number-)| Set the tint of the shape color |
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
### setTintOfShapeColor(number) {#setTintOfShapeColor-number-}
Set the tint of the shape color
```javascript
setTintOfShapeColor(tint: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| tint | number |  |
