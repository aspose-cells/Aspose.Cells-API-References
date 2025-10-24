##LineFormat
Represents all setting of the line.
## LineFormat class
Represents all setting of the line.
```javascript
class LineFormat extends FillFormat;
```
## Constructors
| Constructor | Description |
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
| [getCompoundType()](#getCompoundType--)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the line compound type. |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| <b>@deprecated.</b> Please use the 'compoundType' property instead. Specifies the line compound type. |
| [getDashStyle()](#getDashStyle--)| <b>@deprecated.</b> Please use the 'dashStyle' property instead. Specifies the line dash type. |
| [setDashStyle(MsoLineDashStyle)](#setDashStyle-msolinedashstyle-)| <b>@deprecated.</b> Please use the 'dashStyle' property instead. Specifies the line dash type. |
| [getCapType()](#getCapType--)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| <b>@deprecated.</b> Please use the 'capType' property instead. Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the line join type. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| <b>@deprecated.</b> Please use the 'joinType' property instead. Specifies the line join type. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--)| <b>@deprecated.</b> Please use the 'beginArrowheadStyle' property instead. Gets and sets the begin arrow type of the line. |
| [setBeginArrowheadStyle(MsoArrowheadStyle)](#setBeginArrowheadStyle-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'beginArrowheadStyle' property instead. Gets and sets the begin arrow type of the line. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--)| <b>@deprecated.</b> Please use the 'beginArrowheadWidth' property instead. Gets and sets the begin arrow width type of the line. |
| [setBeginArrowheadWidth(MsoArrowheadWidth)](#setBeginArrowheadWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'beginArrowheadWidth' property instead. Gets and sets the begin arrow width type of the line. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--)| <b>@deprecated.</b> Please use the 'beginArrowheadLength' property instead. Gets and sets the begin arrow length type of the line. |
| [setBeginArrowheadLength(MsoArrowheadLength)](#setBeginArrowheadLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'beginArrowheadLength' property instead. Gets and sets the begin arrow length type of the line. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--)| <b>@deprecated.</b> Please use the 'endArrowheadStyle' property instead. Gets and sets the end arrow type of the line. |
| [setEndArrowheadStyle(MsoArrowheadStyle)](#setEndArrowheadStyle-msoarrowheadstyle-)| <b>@deprecated.</b> Please use the 'endArrowheadStyle' property instead. Gets and sets the end arrow type of the line. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--)| <b>@deprecated.</b> Please use the 'endArrowheadWidth' property instead. Gets and sets the end arrow width type of the line. |
| [setEndArrowheadWidth(MsoArrowheadWidth)](#setEndArrowheadWidth-msoarrowheadwidth-)| <b>@deprecated.</b> Please use the 'endArrowheadWidth' property instead. Gets and sets the end arrow width type of the line. |
| [getEndArrowheadLength()](#getEndArrowheadLength--)| <b>@deprecated.</b> Please use the 'endArrowheadLength' property instead. Gets and sets the end arrow length type of the line. |
| [setEndArrowheadLength(MsoArrowheadLength)](#setEndArrowheadLength-msoarrowheadlength-)| <b>@deprecated.</b> Please use the 'endArrowheadLength' property instead. Gets and sets the end arrow length type of the line. |
| [getWeight()](#getWeight--)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the weight of the line in unit of points. |
| [setWeight(number)](#setWeight-number-)| <b>@deprecated.</b> Please use the 'weight' property instead. Gets or sets the weight of the line in unit of points. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getFillType()](#getFillType--)| <b>@deprecated.</b> Please use the 'fillType' property instead. Gets and sets fill type |
| [setFillType(FillType)](#setFillType-filltype-)| <b>@deprecated.</b> Please use the 'fillType' property instead. Gets and sets fill type |
| [getTransparency()](#getTransparency--)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| <b>@deprecated.</b> Please use the 'transparency' property instead. Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getGradientFill()](#getGradientFill--)| <b>@deprecated.</b> Please use the 'gradientFill' property instead. Gets [GradientFill](../gradientfill/) object. |
| [getTextureFill()](#getTextureFill--)| <b>@deprecated.</b> Please use the 'textureFill' property instead. Gets [TextureFill](../texturefill/) object. |
| [getSolidFill()](#getSolidFill--)| <b>@deprecated.</b> Please use the 'solidFill' property instead. Gets [SolidFill](../solidfill/) object. |
| [getPatternFill()](#getPatternFill--)| <b>@deprecated.</b> Please use the 'patternFill' property instead. Gets [PatternFill](../patternfill/) object. |
| [getGradientColorType()](#getGradientColorType--)| <b>@deprecated.</b> Please use the 'gradientColorType' property instead. Returns the gradient color type for the specified fill. |
| [getGradientStyle()](#getGradientStyle--)| <b>@deprecated.</b> Please use the 'gradientStyle' property instead. Returns the gradient style for the specified fill. |
| [getGradientColor1()](#getGradientColor1--)| <b>@deprecated.</b> Please use the 'gradientColor1' property instead. Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getGradientColor2--)| <b>@deprecated.</b> Please use the 'gradientColor2' property instead. Returns the gradient color 2 for the specified fill. |
| [getGradientDegree()](#getGradientDegree--)| <b>@deprecated.</b> Please use the 'gradientDegree' property instead. Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [getGradientVariant()](#getGradientVariant--)| <b>@deprecated.</b> Please use the 'gradientVariant' property instead. Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [getPresetColor()](#getPresetColor--)| <b>@deprecated.</b> Please use the 'presetColor' property instead. Returns the gradient preset color for the specified fill. |
| [getTexture()](#getTexture--)| <b>@deprecated.</b> Please use the 'texture' property instead. Represents the texture type for the specified fill. |
| [setTexture(TextureType)](#setTexture-texturetype-)| <b>@deprecated.</b> Please use the 'texture' property instead. Represents the texture type for the specified fill. |
| [getPattern()](#getPattern--)| <b>@deprecated.</b> Please use the 'pattern' property instead. Represents an area's display pattern. |
| [setPattern(FillPattern)](#setPattern-fillpattern-)| <b>@deprecated.</b> Please use the 'pattern' property instead. Represents an area's display pattern. |
| [getPictureFormatType()](#getPictureFormatType--)| <b>@deprecated.</b> Please use the 'pictureFormatType' property instead. Gets and sets the picture format type. |
| [setPictureFormatType(FillPictureType)](#setPictureFormatType-fillpicturetype-)| <b>@deprecated.</b> Please use the 'pictureFormatType' property instead. Gets and sets the picture format type. |
| [getScale()](#getScale--)| <b>@deprecated.</b> Please use the 'scale' property instead. Gets and sets the picture format scale. |
| [setScale(number)](#setScale-number-)| <b>@deprecated.</b> Please use the 'scale' property instead. Gets and sets the picture format scale. |
| [getImageData()](#getImageData--)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the picture image data. |
| [setImageData(Uint8Array)](#setImageData-uint8array-)| <b>@deprecated.</b> Please use the 'imageData' property instead. Gets and sets the picture image data. |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, number, Color, number, GradientStyleType, number)](#setTwoColorGradient-color-number-color-number-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setPresetColorGradient(GradientPresetType, GradientStyleType, number)](#setPresetColorGradient-gradientpresettype-gradientstyletype-number-)| Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [getHashCode()](#getHashCode--)| Gets the hash code. |
| [equals(Object)](#equals-object-)| Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object. |
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
### getCompoundType() {#getCompoundType--}
```javascript
getCompoundType() : MsoLineStyle;
```
**Returns**
[MsoLineStyle](../msolinestyle/)
### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}
```javascript
setCompoundType(value: MsoLineStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |
### getDashStyle() {#getDashStyle--}
```javascript
getDashStyle() : MsoLineDashStyle;
```
**Returns**
[MsoLineDashStyle](../msolinedashstyle/)
### setDashStyle(MsoLineDashStyle) {#setDashStyle-msolinedashstyle-}
```javascript
setDashStyle(value: MsoLineDashStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |
### getCapType() {#getCapType--}
```javascript
getCapType() : LineCapType;
```
**Returns**
[LineCapType](../linecaptype/)
### setCapType(LineCapType) {#setCapType-linecaptype-}
```javascript
setCapType(value: LineCapType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |
### getJoinType() {#getJoinType--}
```javascript
getJoinType() : LineJoinType;
```
**Returns**
[LineJoinType](../linejointype/)
### setJoinType(LineJoinType) {#setJoinType-linejointype-}
```javascript
setJoinType(value: LineJoinType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |
### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}
```javascript
getBeginArrowheadStyle() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setBeginArrowheadStyle(MsoArrowheadStyle) {#setBeginArrowheadStyle-msoarrowheadstyle-}
```javascript
setBeginArrowheadStyle(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}
```javascript
getBeginArrowheadWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setBeginArrowheadWidth(MsoArrowheadWidth) {#setBeginArrowheadWidth-msoarrowheadwidth-}
```javascript
setBeginArrowheadWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getBeginArrowheadLength() {#getBeginArrowheadLength--}
```javascript
getBeginArrowheadLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setBeginArrowheadLength(MsoArrowheadLength) {#setBeginArrowheadLength-msoarrowheadlength-}
```javascript
setBeginArrowheadLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getEndArrowheadStyle() {#getEndArrowheadStyle--}
```javascript
getEndArrowheadStyle() : MsoArrowheadStyle;
```
**Returns**
[MsoArrowheadStyle](../msoarrowheadstyle/)
### setEndArrowheadStyle(MsoArrowheadStyle) {#setEndArrowheadStyle-msoarrowheadstyle-}
```javascript
setEndArrowheadStyle(value: MsoArrowheadStyle) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |
### getEndArrowheadWidth() {#getEndArrowheadWidth--}
```javascript
getEndArrowheadWidth() : MsoArrowheadWidth;
```
**Returns**
[MsoArrowheadWidth](../msoarrowheadwidth/)
### setEndArrowheadWidth(MsoArrowheadWidth) {#setEndArrowheadWidth-msoarrowheadwidth-}
```javascript
setEndArrowheadWidth(value: MsoArrowheadWidth) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |
### getEndArrowheadLength() {#getEndArrowheadLength--}
```javascript
getEndArrowheadLength() : MsoArrowheadLength;
```
**Returns**
[MsoArrowheadLength](../msoarrowheadlength/)
### setEndArrowheadLength(MsoArrowheadLength) {#setEndArrowheadLength-msoarrowheadlength-}
```javascript
setEndArrowheadLength(value: MsoArrowheadLength) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |
### getWeight() {#getWeight--}
```javascript
getWeight() : number;
```
### setWeight(number) {#setWeight-number-}
```javascript
setWeight(value: number) : void;
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
### getFillType() {#getFillType--}
```javascript
getFillType() : FillType;
```
**Returns**
[FillType](../filltype/)
### setFillType(FillType) {#setFillType-filltype-}
```javascript
setFillType(value: FillType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillType](../filltype/) | The value to set. |
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
### getGradientFill() {#getGradientFill--}
```javascript
getGradientFill() : GradientFill;
```
**Returns**
[GradientFill](../gradientfill/)
### getTextureFill() {#getTextureFill--}
```javascript
getTextureFill() : TextureFill;
```
**Returns**
[TextureFill](../texturefill/)
### getSolidFill() {#getSolidFill--}
```javascript
getSolidFill() : SolidFill;
```
**Returns**
[SolidFill](../solidfill/)
### getPatternFill() {#getPatternFill--}
```javascript
getPatternFill() : PatternFill;
```
**Returns**
[PatternFill](../patternfill/)
### getGradientColorType() {#getGradientColorType--}
```javascript
getGradientColorType() : GradientColorType;
```
**Returns**
[GradientColorType](../gradientcolortype/)
### getGradientStyle() {#getGradientStyle--}
```javascript
getGradientStyle() : GradientStyleType;
```
**Returns**
[GradientStyleType](../gradientstyletype/)
### getGradientColor1() {#getGradientColor1--}
```javascript
getGradientColor1() : Color;
```
**Returns**
[Color](../color/)
### getGradientColor2() {#getGradientColor2--}
```javascript
getGradientColor2() : Color;
```
**Returns**
[Color](../color/)
**Remarks**
Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.
### getGradientDegree() {#getGradientDegree--}
```javascript
getGradientDegree() : number;
```
**Remarks**
Can only be a value from 0.0 (dark) through 1.0 (light).
### getGradientVariant() {#getGradientVariant--}
```javascript
getGradientVariant() : number;
```
**Remarks**
Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.
### getPresetColor() {#getPresetColor--}
```javascript
getPresetColor() : GradientPresetType;
```
**Returns**
[GradientPresetType](../gradientpresettype/)
### getTexture() {#getTexture--}
```javascript
getTexture() : TextureType;
```
**Returns**
[TextureType](../texturetype/)
### setTexture(TextureType) {#setTexture-texturetype-}
```javascript
setTexture(value: TextureType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextureType](../texturetype/) | The value to set. |
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
### getPictureFormatType() {#getPictureFormatType--}
```javascript
getPictureFormatType() : FillPictureType;
```
**Returns**
[FillPictureType](../fillpicturetype/)
### setPictureFormatType(FillPictureType) {#setPictureFormatType-fillpicturetype-}
```javascript
setPictureFormatType(value: FillPictureType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillPictureType](../fillpicturetype/) | The value to set. |
### getScale() {#getScale--}
```javascript
getScale() : number;
```
### setScale(number) {#setScale-number-}
```javascript
setScale(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getImageData() {#getImageData--}
```javascript
getImageData() : Uint8Array;
```
**Remarks**
If the fill format is not custom texture format, returns null.
### setImageData(Uint8Array) {#setImageData-uint8array-}
```javascript
setImageData(value: Uint8Array) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number[] | The value to set. |
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
### equals(Object) {#equals-object-}
Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object.
```javascript
equals(obj: Object) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The [LineFormat](../lineformat/) object to compare with this instance. |
**Returns**
true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
