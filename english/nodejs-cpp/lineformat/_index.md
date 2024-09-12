---
title: LineFormat
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents all setting of the line.
type: docs
url: /nodejs-cpp/lineformat/
---

## LineFormat class

Represents all setting of the line.

```javascript
class LineFormat extends FillFormat;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(FillFormat)](#constructor-fillformat-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getCompoundType()](#getCompoundType--)| Specifies the line compound type. |
| [setCompoundType(MsoLineStyle)](#setCompoundType-msolinestyle-)| Specifies the line compound type. |
| [getDashStyle()](#getDashStyle--)| Specifies the line dash type. |
| [setDashStyle(MsoLineDashStyle)](#setDashStyle-msolinedashstyle-)| Specifies the line dash type. |
| [getCapType()](#getCapType--)| Specifies the ending caps. |
| [setCapType(LineCapType)](#setCapType-linecaptype-)| Specifies the ending caps. |
| [getJoinType()](#getJoinType--)| Specifies the line join type. |
| [setJoinType(LineJoinType)](#setJoinType-linejointype-)| Specifies the line join type. |
| [getBeginArrowheadStyle()](#getBeginArrowheadStyle--)| Gets and sets the begin arrow type of the line. |
| [setBeginArrowheadStyle(MsoArrowheadStyle)](#setBeginArrowheadStyle-msoarrowheadstyle-)| Gets and sets the begin arrow type of the line. |
| [getBeginArrowheadWidth()](#getBeginArrowheadWidth--)| Gets and sets the begin arrow width type of the line. |
| [setBeginArrowheadWidth(MsoArrowheadWidth)](#setBeginArrowheadWidth-msoarrowheadwidth-)| Gets and sets the begin arrow width type of the line. |
| [getBeginArrowheadLength()](#getBeginArrowheadLength--)| Gets and sets the begin arrow length type of the line. |
| [setBeginArrowheadLength(MsoArrowheadLength)](#setBeginArrowheadLength-msoarrowheadlength-)| Gets and sets the begin arrow length type of the line. |
| [getEndArrowheadStyle()](#getEndArrowheadStyle--)| Gets and sets the end arrow type of the line. |
| [setEndArrowheadStyle(MsoArrowheadStyle)](#setEndArrowheadStyle-msoarrowheadstyle-)| Gets and sets the end arrow type of the line. |
| [getEndArrowheadWidth()](#getEndArrowheadWidth--)| Gets and sets the end arrow width type of the line. |
| [setEndArrowheadWidth(MsoArrowheadWidth)](#setEndArrowheadWidth-msoarrowheadwidth-)| Gets and sets the end arrow width type of the line. |
| [getEndArrowheadLength()](#getEndArrowheadLength--)| Gets and sets the end arrow length type of the line. |
| [setEndArrowheadLength(MsoArrowheadLength)](#setEndArrowheadLength-msoarrowheadlength-)| Gets and sets the end arrow length type of the line. |
| [getWeight()](#getWeight--)| Gets or sets the weight of the line in unit of points. |
| [setWeight(number)](#setWeight-number-)| Gets or sets the weight of the line in unit of points. |
| [getHashCode()](#getHashCode--)| Gets the hash code. |
| [equals(object)](#equals-object-)| Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
| [getFillType()](#getFillType--)| Gets and sets fill type |
| [setFillType(FillType)](#setFillType-filltype-)| Gets and sets fill type |
| [getTransparency()](#getTransparency--)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTransparency(number)](#setTransparency-number-)| Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getGradientFill()](#getGradientFill--)| Gets [GradientFill](../gradientfill/) object. |
| [getTextureFill()](#getTextureFill--)| Gets [TextureFill](../texturefill/) object. |
| [getSolidFill()](#getSolidFill--)| Gets [SolidFill](../solidfill/) object. |
| [getPatternFill()](#getPatternFill--)| Gets [PatternFill](../patternfill/) object. |
| [getGradientColorType()](#getGradientColorType--)| Returns the gradient color type for the specified fill. |
| [getGradientStyle()](#getGradientStyle--)| Returns the gradient style for the specified fill. |
| [getGradientColor1()](#getGradientColor1--)| Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getGradientColor2--)| Returns the gradient color 2 for the specified fill. |
| [getGradientDegree()](#getGradientDegree--)| Returns the gradient degree for the specified fill. Only applies for Excel 2007. |
| [getGradientVariant()](#getGradientVariant--)| Returns the gradient variant for the specified fill. Only applies for Excel 2007. |
| [getPresetColor()](#getPresetColor--)| Returns the gradient preset color for the specified fill. |
| [getTexture()](#getTexture--)| Represents the texture type for the specified fill. |
| [setTexture(TextureType)](#setTexture-texturetype-)| Represents the texture type for the specified fill. |
| [getPattern()](#getPattern--)| Represents an area's display pattern. |
| [setPattern(FillPattern)](#setPattern-fillpattern-)| Represents an area's display pattern. |
| [getPictureFormatType()](#getPictureFormatType--)| Gets and sets the picture format type. |
| [setPictureFormatType(FillPictureType)](#setPictureFormatType-fillpicturetype-)| Gets and sets the picture format type. |
| [getScale()](#getScale--)| Gets and sets the picture format scale. |
| [setScale(number)](#setScale-number-)| Gets and sets the picture format scale. |
| [getImageData()](#getImageData--)| Gets and sets the picture image data. |
| [setImageData(number[])](#setImageData-numberarray-)| Gets and sets the picture image data. |
| [setOneColorGradient(Color, number, GradientStyleType, number)](#setOneColorGradient-color-number-gradientstyletype-number-)| Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, Color, GradientStyleType, number)](#setTwoColorGradient-color-color-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(Color, number, Color, number, GradientStyleType, number)](#setTwoColorGradient-color-number-color-number-gradientstyletype-number-)| Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setPresetColorGradient(GradientPresetType, GradientStyleType, number)](#setPresetColorGradient-gradientpresettype-gradientstyletype-number-)| Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |


### constructor(FillFormat) {#constructor-fillformat-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: FillFormat);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | FillFormat | The parent object. |

### getCompoundType() {#getCompoundType--}

Specifies the line compound type.

```javascript
getCompoundType() : MsoLineStyle;
```


**Returns**

[MsoLineStyle](../msolinestyle/)

### setCompoundType(MsoLineStyle) {#setCompoundType-msolinestyle-}

Specifies the line compound type.

```javascript
setCompoundType(value: MsoLineStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineStyle](../msolinestyle/) | The value to set. |

### getDashStyle() {#getDashStyle--}

Specifies the line dash type.

```javascript
getDashStyle() : MsoLineDashStyle;
```


**Returns**

[MsoLineDashStyle](../msolinedashstyle/)

### setDashStyle(MsoLineDashStyle) {#setDashStyle-msolinedashstyle-}

Specifies the line dash type.

```javascript
setDashStyle(value: MsoLineDashStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoLineDashStyle](../msolinedashstyle/) | The value to set. |

### getCapType() {#getCapType--}

Specifies the ending caps.

```javascript
getCapType() : LineCapType;
```


**Returns**

[LineCapType](../linecaptype/)

### setCapType(LineCapType) {#setCapType-linecaptype-}

Specifies the ending caps.

```javascript
setCapType(value: LineCapType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineCapType](../linecaptype/) | The value to set. |

### getJoinType() {#getJoinType--}

Specifies the line join type.

```javascript
getJoinType() : LineJoinType;
```


**Returns**

[LineJoinType](../linejointype/)

### setJoinType(LineJoinType) {#setJoinType-linejointype-}

Specifies the line join type.

```javascript
setJoinType(value: LineJoinType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [LineJoinType](../linejointype/) | The value to set. |

### getBeginArrowheadStyle() {#getBeginArrowheadStyle--}

Gets and sets the begin arrow type of the line.

```javascript
getBeginArrowheadStyle() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setBeginArrowheadStyle(MsoArrowheadStyle) {#setBeginArrowheadStyle-msoarrowheadstyle-}

Gets and sets the begin arrow type of the line.

```javascript
setBeginArrowheadStyle(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getBeginArrowheadWidth() {#getBeginArrowheadWidth--}

Gets and sets the begin arrow width type of the line.

```javascript
getBeginArrowheadWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setBeginArrowheadWidth(MsoArrowheadWidth) {#setBeginArrowheadWidth-msoarrowheadwidth-}

Gets and sets the begin arrow width type of the line.

```javascript
setBeginArrowheadWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getBeginArrowheadLength() {#getBeginArrowheadLength--}

Gets and sets the begin arrow length type of the line.

```javascript
getBeginArrowheadLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setBeginArrowheadLength(MsoArrowheadLength) {#setBeginArrowheadLength-msoarrowheadlength-}

Gets and sets the begin arrow length type of the line.

```javascript
setBeginArrowheadLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getEndArrowheadStyle() {#getEndArrowheadStyle--}

Gets and sets the end arrow type of the line.

```javascript
getEndArrowheadStyle() : MsoArrowheadStyle;
```


**Returns**

[MsoArrowheadStyle](../msoarrowheadstyle/)

### setEndArrowheadStyle(MsoArrowheadStyle) {#setEndArrowheadStyle-msoarrowheadstyle-}

Gets and sets the end arrow type of the line.

```javascript
setEndArrowheadStyle(value: MsoArrowheadStyle) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadStyle](../msoarrowheadstyle/) | The value to set. |

### getEndArrowheadWidth() {#getEndArrowheadWidth--}

Gets and sets the end arrow width type of the line.

```javascript
getEndArrowheadWidth() : MsoArrowheadWidth;
```


**Returns**

[MsoArrowheadWidth](../msoarrowheadwidth/)

### setEndArrowheadWidth(MsoArrowheadWidth) {#setEndArrowheadWidth-msoarrowheadwidth-}

Gets and sets the end arrow width type of the line.

```javascript
setEndArrowheadWidth(value: MsoArrowheadWidth) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadWidth](../msoarrowheadwidth/) | The value to set. |

### getEndArrowheadLength() {#getEndArrowheadLength--}

Gets and sets the end arrow length type of the line.

```javascript
getEndArrowheadLength() : MsoArrowheadLength;
```


**Returns**

[MsoArrowheadLength](../msoarrowheadlength/)

### setEndArrowheadLength(MsoArrowheadLength) {#setEndArrowheadLength-msoarrowheadlength-}

Gets and sets the end arrow length type of the line.

```javascript
setEndArrowheadLength(value: MsoArrowheadLength) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [MsoArrowheadLength](../msoarrowheadlength/) | The value to set. |

### getWeight() {#getWeight--}

Gets or sets the weight of the line in unit of points.

```javascript
getWeight() : number;
```


### setWeight(number) {#setWeight-number-}

Gets or sets the weight of the line in unit of points.

```javascript
setWeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHashCode() {#getHashCode--}

Gets the hash code.

```javascript
getHashCode() : number;
```


### equals(object) {#equals-object-}

Determines whether this instance has the same value as another specified [LineFormat](../lineformat/) object.

```javascript
equals(obj: object) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | object | The [LineFormat](../lineformat/) object to compare with this instance. |

**Returns**

true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.

### isNull() {#isNull--}

Checks whether the implementation object is null.

```javascript
isNull() : boolean;
```


### getFillType() {#getFillType--}

Gets and sets fill type

```javascript
getFillType() : FillType;
```


**Returns**

[FillType](../filltype/)

### setFillType(FillType) {#setFillType-filltype-}

Gets and sets fill type

```javascript
setFillType(value: FillType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillType](../filltype/) | The value to set. |

### getTransparency() {#getTransparency--}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
getTransparency() : number;
```


### setTransparency(number) {#setTransparency-number-}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

```javascript
setTransparency(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getGradientFill() {#getGradientFill--}

Gets [GradientFill](../gradientfill/) object.

```javascript
getGradientFill() : GradientFill;
```


**Returns**

[GradientFill](../gradientfill/)

### getTextureFill() {#getTextureFill--}

Gets [TextureFill](../texturefill/) object.

```javascript
getTextureFill() : TextureFill;
```


**Returns**

[TextureFill](../texturefill/)

### getSolidFill() {#getSolidFill--}

Gets [SolidFill](../solidfill/) object.

```javascript
getSolidFill() : SolidFill;
```


**Returns**

[SolidFill](../solidfill/)

### getPatternFill() {#getPatternFill--}

Gets [PatternFill](../patternfill/) object.

```javascript
getPatternFill() : PatternFill;
```


**Returns**

[PatternFill](../patternfill/)

### getGradientColorType() {#getGradientColorType--}

Returns the gradient color type for the specified fill.

```javascript
getGradientColorType() : GradientColorType;
```


**Returns**

[GradientColorType](../gradientcolortype/)

### getGradientStyle() {#getGradientStyle--}

Returns the gradient style for the specified fill.

```javascript
getGradientStyle() : GradientStyleType;
```


**Returns**

[GradientStyleType](../gradientstyletype/)

### getGradientColor1() {#getGradientColor1--}

Returns the gradient color 1 for the specified fill.

```javascript
getGradientColor1() : Color;
```


**Returns**

[Color](../color/)

### getGradientColor2() {#getGradientColor2--}

Returns the gradient color 2 for the specified fill.

```javascript
getGradientColor2() : Color;
```


**Returns**

[Color](../color/)

**Remarks**

Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

### getGradientDegree() {#getGradientDegree--}

Returns the gradient degree for the specified fill. Only applies for Excel 2007.

```javascript
getGradientDegree() : number;
```


**Remarks**

Can only be a value from 0.0 (dark) through 1.0 (light).

### getGradientVariant() {#getGradientVariant--}

Returns the gradient variant for the specified fill. Only applies for Excel 2007.

```javascript
getGradientVariant() : number;
```


**Remarks**

Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

### getPresetColor() {#getPresetColor--}

Returns the gradient preset color for the specified fill.

```javascript
getPresetColor() : GradientPresetType;
```


**Returns**

[GradientPresetType](../gradientpresettype/)

### getTexture() {#getTexture--}

Represents the texture type for the specified fill.

```javascript
getTexture() : TextureType;
```


**Returns**

[TextureType](../texturetype/)

### setTexture(TextureType) {#setTexture-texturetype-}

Represents the texture type for the specified fill.

```javascript
setTexture(value: TextureType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextureType](../texturetype/) | The value to set. |

### getPattern() {#getPattern--}

Represents an area's display pattern.

```javascript
getPattern() : FillPattern;
```


**Returns**

[FillPattern](../fillpattern/)

### setPattern(FillPattern) {#setPattern-fillpattern-}

Represents an area's display pattern.

```javascript
setPattern(value: FillPattern) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillPattern](../fillpattern/) | The value to set. |

### getPictureFormatType() {#getPictureFormatType--}

Gets and sets the picture format type.

```javascript
getPictureFormatType() : FillPictureType;
```


**Returns**

[FillPictureType](../fillpicturetype/)

### setPictureFormatType(FillPictureType) {#setPictureFormatType-fillpicturetype-}

Gets and sets the picture format type.

```javascript
setPictureFormatType(value: FillPictureType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FillPictureType](../fillpicturetype/) | The value to set. |

### getScale() {#getScale--}

Gets and sets the picture format scale.

```javascript
getScale() : number;
```


### setScale(number) {#setScale-number-}

Gets and sets the picture format scale.

```javascript
setScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getImageData() {#getImageData--}

Gets and sets the picture image data.

```javascript
getImageData() : number[];
```


**Returns**

number[]

**Remarks**

If the fill format is not custom texture format, returns null.

### setImageData(number[]) {#setImageData-numberarray-}

Gets and sets the picture image data.

```javascript
setImageData(value: number[]) : void;
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


