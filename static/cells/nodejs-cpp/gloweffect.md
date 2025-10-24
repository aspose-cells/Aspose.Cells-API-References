##GlowEffect
This class specifies a glow effect in which a color blurred outline is added outside the edges of the object.
## GlowEffect class
This class specifies a glow effect, in which a color blurred outline is added outside the edges of the object.
```javascript
class GlowEffect;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [color](#color--)| CellsColor | Gets the color of the glow effect. |
| [size](#size--)| number | Gets and sets the radius of the glow, in unit of points. |
| [transparency](#transparency--)| number | Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets the color of the glow effect. |
| [setColor(CellsColor)](#setColor-cellscolor-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets the color of the glow effect. |
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the radius of the glow, in unit of points. |
| [setSize(number)](#setSize-number-)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the radius of the glow, in unit of points. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### color {#color--}
Gets the color of the glow effect.
```javascript
color : CellsColor;
```
### size {#size--}
Gets and sets the radius of the glow, in unit of points.
```javascript
size : number;
```
### transparency {#transparency--}
Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear).
```javascript
transparency : number;
```
### getColor() {#getColor--}
```javascript
getColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setColor(CellsColor) {#setColor-cellscolor-}
```javascript
setColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
### getSize() {#getSize--}
```javascript
getSize() : number;
```
### setSize(number) {#setSize-number-}
```javascript
setSize(value: number) : void;
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
