##LineFormat
Represents all setting of the line.
## LineFormat class
Represents all setting of the line.
```javascript
class LineFormat extends FillFormat;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor(FillFormat)](#constructor-fillformat-)| Constructs from a parent object convertible to this. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [compoundType](#compoundType--)| MsoLineStyle | Specifies the line compound type. |
| [dashStyle](#dashStyle--)| MsoLineDashStyle | Specifies the line dash type. |
| [capType](#capType--)| LineCapType | Specifies the ending caps. |
| [joinType](#joinType--)| LineJoinType | Specifies the line join type. |
| [beginArrowheadStyle](#beginArrowheadStyle--)| MsoArrowheadStyle | Gets and sets the begin arrow type of the line. |
| [beginArrowheadWidth](#beginArrowheadWidth--)| MsoArrowheadWidth | Gets and sets the begin arrow width type of the line. |
| [beginArrowheadLength](#beginArrowheadLength--)| MsoArrowheadLength | Gets and sets the begin arrow length type of the line. |
| [endArrowheadStyle](#endArrowheadStyle--)| MsoArrowheadStyle | Gets and sets the end arrow type of the line. |
| [endArrowheadWidth](#endArrowheadWidth--)| MsoArrowheadWidth | Gets and sets the end arrow width type of the line. |
| [endArrowheadLength](#endArrowheadLength--)| MsoArrowheadLength | Gets and sets the end arrow length type of the line. |
| [weight](#weight--)| number | Gets or sets the weight of the line in unit of points. |
| [fillType](#fillType--)| FillType | Gets and sets fill type |
| [transparency](#transparency--)| number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [gradientFill](#gradientFill--)| GradientFill | Readonly. Gets [GradientFill](../gradientfill/) object. |
| [textureFill](#textureFill--)| TextureFill | Readonly. Gets [TextureFill](../texturefill/) object. |
| [solidFill](#solidFill--)| SolidFill | Readonly. Gets [SolidFill](../solidfill/) object. |
| [patternFill](#patternFill--)| PatternFill | Readonly. Gets [PatternFill](../patternfill/) object. |
| [gradientColorType](#gradientColorType--)| GradientColorType | Readonly. Returns the gradient color type for the specified fill. |
| [gradientStyle](#gradientStyle--)| GradientStyleType | Readonly. Returns the gradient style for the specified fill. |
| [gradientColor1](#gradientColor1--)| Color | Readonly. Returns the gradient color 1 for the specified fill. |
| [gradientColor2](#gradientColor2--)| Color | Readonly. Returns the gradient color 2 for the specified fill. |
| [gradientDegree](#gradientDegree--)| number | Readonly. Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [gradientVariant](#gradientVariant--)| number | Readonly. Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [presetColor](#presetColor--)| GradientPresetType | Readonly. Returns the gradient preset color for the specified fill. |
| [texture](#texture--)| TextureType | Represents the texture type for the specified fill. |
| [pattern](#pattern--)| FillPattern | Represents an area's display pattern. |
| [pictureFormatType](#pictureFormatType--)| FillPictureType | Gets and sets the picture format type. |
| [scale](#scale--)| number | Gets and sets the picture format scale. |
| [imageData](#imageData--)| Uint8Array | Gets and sets the picture image data. |
## Methods
| Method | Description |
| --- | --- |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, number, Color, number, GradientStyleType, number)](#setTwoColorGradient-color-number-color-number-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setPresetColorGradient(GradientPresetType, GradientStyleType, number)](#setPresetColorGradient-gradientpresettype-gradientstyletype-number-)| Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [getHashCode()](#getHashCode--)| Gets the hash code. |
| [equals(VObject)](#equals-vobject-)| Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object. |
### constructor(FillFormat) {#constructor-fillformat-}
Constructs from a parent object convertible to this.
```javascript
constructor(obj: FillFormat);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FillFormat | The parent object. |
### compoundType {#compoundType--}
Specifies the line compound type.
```javascript
compoundType : MsoLineStyle;
```
### dashStyle {#dashStyle--}
Specifies the line dash type.
```javascript
dashStyle : MsoLineDashStyle;
```
### capType {#capType--}
Specifies the ending caps.
```javascript
capType : LineCapType;
```
### joinType {#joinType--}
Specifies the line join type.
```javascript
joinType : LineJoinType;
```
### beginArrowheadStyle {#beginArrowheadStyle--}
Gets and sets the begin arrow type of the line.
```javascript
beginArrowheadStyle : MsoArrowheadStyle;
```
### beginArrowheadWidth {#beginArrowheadWidth--}
Gets and sets the begin arrow width type of the line.
```javascript
beginArrowheadWidth : MsoArrowheadWidth;
```
### beginArrowheadLength {#beginArrowheadLength--}
Gets and sets the begin arrow length type of the line.
```javascript
beginArrowheadLength : MsoArrowheadLength;
```
### endArrowheadStyle {#endArrowheadStyle--}
Gets and sets the end arrow type of the line.
```javascript
endArrowheadStyle : MsoArrowheadStyle;
```
### endArrowheadWidth {#endArrowheadWidth--}
Gets and sets the end arrow width type of the line.
```javascript
endArrowheadWidth : MsoArrowheadWidth;
```
### endArrowheadLength {#endArrowheadLength--}
Gets and sets the end arrow length type of the line.
```javascript
endArrowheadLength : MsoArrowheadLength;
```
### weight {#weight--}
Gets or sets the weight of the line in unit of points.
```javascript
weight : number;
```
### fillType {#fillType--}
Gets and sets fill type
```javascript
fillType : FillType;
```
### transparency {#transparency--}
Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).
```javascript
transparency : number;
```
### gradientFill {#gradientFill--}
Readonly. Gets [GradientFill](../gradientfill/) object.
```javascript
gradientFill : GradientFill;
```
### textureFill {#textureFill--}
Readonly. Gets [TextureFill](../texturefill/) object.
```javascript
textureFill : TextureFill;
```
### solidFill {#solidFill--}
Readonly. Gets [SolidFill](../solidfill/) object.
```javascript
solidFill : SolidFill;
```
### patternFill {#patternFill--}
Readonly. Gets [PatternFill](../patternfill/) object.
```javascript
patternFill : PatternFill;
```
### gradientColorType {#gradientColorType--}
Readonly. Returns the gradient color type for the specified fill.
```javascript
gradientColorType : GradientColorType;
```
### gradientStyle {#gradientStyle--}
Readonly. Returns the gradient style for the specified fill.
```javascript
gradientStyle : GradientStyleType;
```
### gradientColor1 {#gradientColor1--}
Readonly. Returns the gradient color 1 for the specified fill.
```javascript
gradientColor1 : Color;
```
### gradientColor2 {#gradientColor2--}
Readonly. Returns the gradient color 2 for the specified fill.
```javascript
gradientColor2 : Color;
```
**Remarks**
Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.
### gradientDegree {#gradientDegree--}
Readonly. Returns the gradient degree for the specified fill. Only applies for Excel 2007.
```javascript
gradientDegree : number;
```
**Remarks**
Can only be a value from 0.0 (dark) through 1.0 (light).
### gradientVariant {#gradientVariant--}
Readonly. Returns the gradient variant for the specified fill. Only applies for Excel 2007.
```javascript
gradientVariant : number;
```
**Remarks**
Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.
### presetColor {#presetColor--}
Readonly. Returns the gradient preset color for the specified fill.
```javascript
presetColor : GradientPresetType;
```
### texture {#texture--}
Represents the texture type for the specified fill.
```javascript
texture : TextureType;
```
### pattern {#pattern--}
Represents an area's display pattern.
```javascript
pattern : FillPattern;
```
### pictureFormatType {#pictureFormatType--}
Gets and sets the picture format type.
```javascript
pictureFormatType : FillPictureType;
```
### scale {#scale--}
Gets and sets the picture format scale.
```javascript
scale : number;
```
### imageData {#imageData--}
Gets and sets the picture image data.
```javascript
imageData : Uint8Array;
```
**Remarks**
If the fill format is not custom texture format, returns null.
### setOneColorGradient(Color, number, GradientStyleType, number) {#setOneColorGradient-color-number-gradientstyletype-number-}
Sets the specified fill to a one-color gradient. Only applies for Excel 2007.
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
### setTwoColorGradient(Color, Color, GradientStyleType, number) {#setTwoColorGradient-color-color-gradientstyletype-number-}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```javascript
setTwoColorGradient(color1: Color, color2: Color, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) | One gradient color. |
| color2 | [Color](../color/) | Two gradient color. |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setTwoColorGradient(Color, number, Color, number, GradientStyleType, number) {#setTwoColorGradient-color-number-color-number-gradientstyletype-number-}
Sets the specified fill to a two-color gradient. Only applies for Excel 2007.
```javascript
setTwoColorGradient(color1: Color, transparency1: number, color2: Color, transparency2: number, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| color1 | [Color](../color/) | One gradient color. |
| transparency1 | number | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | [Color](../color/) | Two gradient color. |
| transparency2 | number | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### setPresetColorGradient(GradientPresetType, GradientStyleType, number) {#setPresetColorGradient-gradientpresettype-gradientstyletype-number-}
Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.
```javascript
setPresetColorGradient(presetColor: GradientPresetType, style: GradientStyleType, variant: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | [GradientPresetType](../gradientpresettype/) | Preset color type |
| style | [GradientStyleType](../gradientstyletype/) | Gradient shading style. |
| variant | number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
### getHashCode() {#getHashCode--}
Gets the hash code.
```javascript
getHashCode() : number;
```
### equals(VObject) {#equals-vobject-}
Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object.
```javascript
equals(obj: VObject) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject | The [LineFormat](../lineformat/) object to compare with this instance. |
**Returns**
true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
