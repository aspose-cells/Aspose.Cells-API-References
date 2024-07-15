---
title: FillFormat
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents fill formatting for a shape.
type: docs
url: /nodejs-cpp/fillformat/
---

## FillFormat class

Encapsulates the object that represents fill formatting for a shape.

```javascript
class FillFormat;
```


## Methods

| Method | Description |
| --- | --- |
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
| [getHashCode()](#getHashCode--)| Gets the hash code. |


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

### getHashCode() {#getHashCode--}

Gets the hash code.

```javascript
getHashCode() : number;
```



