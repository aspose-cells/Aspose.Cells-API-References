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
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. |
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
