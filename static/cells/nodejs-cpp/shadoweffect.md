##ShadowEffect
This class specifies the shadow effect of the chart element or shape.
## ShadowEffect class
This class specifies the shadow effect of the chart element or shape.
```javascript
class ShadowEffect;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [presetType](#presetType--)| PresetShadowType | Gets and sets the preset shadow type of the shadow. |
| [color](#color--)| CellsColor | Gets and sets the color of the shadow. |
| [transparency](#transparency--)| number | Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
| [size](#size--)| number | Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow. |
| [blur](#blur--)| number | Gets and sets the blur of the shadow. Range from 0 to 100 points. |
| [angle](#angle--)| number | Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [distance](#distance--)| number | Gets and sets the distance of the shadow. Range from 0 to 200 points. |
## Methods
| Method | Description |
| --- | --- |
| [getPresetType()](#getPresetType--)| <b>@deprecated.</b> Please use the 'presetType' property instead. Gets and sets the preset shadow type of the shadow. |
| [setPresetType(PresetShadowType)](#setPresetType-presetshadowtype-)| <b>@deprecated.</b> Please use the 'presetType' property instead. Gets and sets the preset shadow type of the shadow. |
| [getColor()](#getColor--)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the color of the shadow. |
| [setColor(CellsColor)](#setColor-cellscolor-)| <b>@deprecated.</b> Please use the 'color' property instead. Gets and sets the color of the shadow. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear). |
| [getSize()](#getSize--)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow. |
| [setSize(number)](#setSize-number-)| <b>@deprecated.</b> Please use the 'size' property instead. Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow. |
| [getBlur()](#getBlur--)| <b>@deprecated.</b> Please use the 'blur' property instead. Gets and sets the blur of the shadow. Range from 0 to 100 points. |
| [setBlur(number)](#setBlur-number-)| <b>@deprecated.</b> Please use the 'blur' property instead. Gets and sets the blur of the shadow. Range from 0 to 100 points. |
| [getAngle()](#getAngle--)| <b>@deprecated.</b> Please use the 'angle' property instead. Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [setAngle(number)](#setAngle-number-)| <b>@deprecated.</b> Please use the 'angle' property instead. Gets and sets the lighting angle. Range from 0 to 359.9 degrees. |
| [getDistance()](#getDistance--)| <b>@deprecated.</b> Please use the 'distance' property instead. Gets and sets the distance of the shadow. Range from 0 to 200 points. |
| [setDistance(number)](#setDistance-number-)| <b>@deprecated.</b> Please use the 'distance' property instead. Gets and sets the distance of the shadow. Range from 0 to 200 points. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### presetType {#presetType--}
Gets and sets the preset shadow type of the shadow.
```javascript
presetType : PresetShadowType;
```
### color {#color--}
Gets and sets the color of the shadow.
```javascript
color : CellsColor;
```
### transparency {#transparency--}
Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear).
```javascript
transparency : number;
```
### size {#size--}
Gets and sets the size of the shadow. Range from 0 to 2.0. Meaningless in inner shadow.
```javascript
size : number;
```
### blur {#blur--}
Gets and sets the blur of the shadow. Range from 0 to 100 points.
```javascript
blur : number;
```
### angle {#angle--}
Gets and sets the lighting angle. Range from 0 to 359.9 degrees.
```javascript
angle : number;
```
### distance {#distance--}
Gets and sets the distance of the shadow. Range from 0 to 200 points.
```javascript
distance : number;
```
### getPresetType() {#getPresetType--}
```javascript
getPresetType() : PresetShadowType;
```
**Returns**
[PresetShadowType](../presetshadowtype/)
### setPresetType(PresetShadowType) {#setPresetType-presetshadowtype-}
```javascript
setPresetType(value: PresetShadowType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PresetShadowType](../presetshadowtype/) | The value to set. |
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
### getBlur() {#getBlur--}
```javascript
getBlur() : number;
```
### setBlur(number) {#setBlur-number-}
```javascript
setBlur(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getAngle() {#getAngle--}
```javascript
getAngle() : number;
```
### setAngle(number) {#setAngle-number-}
```javascript
setAngle(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getDistance() {#getDistance--}
```javascript
getDistance() : number;
```
### setDistance(number) {#setDistance-number-}
```javascript
setDistance(value: number) : void;
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
