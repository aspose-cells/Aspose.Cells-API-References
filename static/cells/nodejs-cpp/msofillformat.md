##MsoFillFormat
Represents fill formatting for a shape.
## MsoFillFormat class
Represents fill formatting for a shape.
```javascript
class MsoFillFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [foreColor](#foreColor--)| Color | Gets and sets the fill fore color. |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [backColor](#backColor--)| Color | Gets and sets the file back color. |
| [imageData](#imageData--)| Uint8Array | Gets and sets the Texture and Picture fill data. |
| [texture](#texture--)| TextureType | Readonly. Gets the texture fill type. |
| [isVisible](#isVisible--)| boolean | Indicates whether there is fill. |
## Methods
| Method | Description |
| --- | --- |
| [getForeColor()](#getForeColor--)| <b>@deprecated.</b> Please use the 'foreColor' property instead. Gets and sets the fill fore color. |
| [setForeColor(Color)](#setForeColor-color-)| <b>@deprecated.</b> Please use the 'foreColor' property instead. Gets and sets the fill fore color. |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [getBackColor()](#getBackColor--)| <b>@deprecated.</b> Please use the 'backColor' property instead. Gets and sets the file back color. |
| [setBackColor(Color)](#setBackColor-color-)| <b>@deprecated.</b> Please use the 'backColor' property instead. Gets and sets the file back color. |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the Texture and Picture fill data. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the Texture and Picture fill data. |
| [getTexture()](#getTexture--)| <b>@deprecated.</b> Please use the 'texture' property instead. Gets the texture fill type. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether there is fill. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Indicates whether there is fill. |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### foreColor {#foreColor--}
Gets and sets the fill fore color.
```javascript
foreColor : Color;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### backColor {#backColor--}
Gets and sets the file back color.
```javascript
backColor : Color;
```
### imageData {#imageData--}
Gets and sets the Texture and Picture fill data.
```javascript
imageData : Uint8Array;
```
### texture {#texture--}
Readonly. Gets the texture fill type.
```javascript
texture : TextureType;
```
### isVisible {#isVisible--}
Indicates whether there is fill.
```javascript
isVisible : boolean;
```
### getForeColor() {#getForeColor--}
```javascript
getForeColor() : Color;
```
**Returns**
[Color](../color/)
### setForeColor(Color) {#setForeColor-color-}
```javascript
setForeColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
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
### getBackColor() {#getBackColor--}
```javascript
getBackColor() : Color;
```
**Returns**
[Color](../color/)
### setBackColor(Color) {#setBackColor-color-}
```javascript
setBackColor(value: Color) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../color/) | The value to set. |
### getImageData() {#getImageData--}
```javascript
getImageData() : Uint8Array;
```
### setImageData(Uint8Array) {#setImageData-uint8array-}
```javascript
setImageData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
### getTexture() {#getTexture--}
```javascript
getTexture() : TextureType;
```
**Returns**
[TextureType](../texturetype/)
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### setOneColorGradient(Color, number, GradientStyleType, number) {#setOneColorGradient-color-number-gradientstyletype-number-}
Sets the specified fill to a one-color gradient.
```javascript
setOneColorGradient(color: Color, degree: number, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color | [Color](../color/) | One gradient color. |
| degree | number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
