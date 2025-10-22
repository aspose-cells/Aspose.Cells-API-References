##SolidFill
Encapsulates the object that represents solid fill format
## SolidFill class
Encapsulates the object that represents solid fill format
```javascript
class SolidFill;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [color](#color--)| Color | Gets or sets the [Color](../color/). |
| [cellsColor](#cellsColor--)| CellsColor | Gets and sets the [CellsColor](../cellscolor/) object. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/). |
| [setColor(Color)](#setColor-color-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets or sets the [Color](../color/). |
| [getCellsColor()](#getCellsColor--)| <b>@deprecated.</b> Please use the 'cellsColor' property instead. Gets and sets the [CellsColor](../cellscolor/) object. |
| [setCellsColor(CellsColor)](#setCellsColor-cellscolor-)| <b>@deprecated.</b> Please use the 'cellsColor' property instead. Gets and sets the [CellsColor](../cellscolor/) object. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getHashCode()](#getHashCode--)| Gets the hash code. |
| [equals(Object)](#equals-object-)|  |
### color {#color--}
Gets or sets the [Color](../color/).
```javascript
color : Color;
```
### cellsColor {#cellsColor--}
Gets and sets the [CellsColor](../cellscolor/) object.
```javascript
cellsColor : CellsColor;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
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
### getCellsColor() {#getCellsColor--}
```javascript
getCellsColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
### setCellsColor(CellsColor) {#setCellsColor-cellscolor-}
```javascript
setCellsColor(value: CellsColor) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [CellsColor](../cellscolor/) | The value to set. |
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
### getHashCode() {#getHashCode--}
Gets the hash code.
```javascript
getHashCode() : number;
```
### equals(Object) {#equals-object-}
```javascript
equals(obj: Object) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |
