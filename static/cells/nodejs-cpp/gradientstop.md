##GradientStop
Represents the gradient stop.
## GradientStop class
Represents the gradient stop.
```javascript
class GradientStop;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [position](#position--)| number | The position of the stop. |
| [cellsColor](#cellsColor--)| CellsColor | Readonly. Gets the color of this gradient stop. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
## Methods
| Method | Description |
| --- | --- |
| [getPosition()](#getPosition--)| <b>@deprecated.</b> Please use the 'position' property instead. The position of the stop. |
| [setPosition(number)](#setPosition-number-)| <b>@deprecated.</b> Please use the 'position' property instead. The position of the stop. |
| [getCellsColor()](#getCellsColor--)| <b>@deprecated.</b> Please use the 'cellsColor' property instead. Gets the color of this gradient stop. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### position {#position--}
The position of the stop.
```javascript
position : number;
```
### cellsColor {#cellsColor--}
Readonly. Gets the color of this gradient stop.
```javascript
cellsColor : CellsColor;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### getPosition() {#getPosition--}
```javascript
getPosition() : number;
```
### setPosition(number) {#setPosition-number-}
```javascript
setPosition(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getCellsColor() {#getCellsColor--}
```javascript
getCellsColor() : CellsColor;
```
**Returns**
[CellsColor](../cellscolor/)
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
