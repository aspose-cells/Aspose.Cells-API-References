---
title: "LineFormat"
linktitle: "LineFormat"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents all setting of the line."
type: docs
weight: 2060
url: /nodejs/aspose.cells/lineformat/
---

## LineFormat class

Represents all setting of the line.

## Methods

| Name | Description |
| --- | --- |
| [equals(obj)](#equals) | Determines whether this instance has the same value as another specified LineFormat object. |
| [getBeginArrowheadLength()](#getbeginarrowheadlength) | Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [getBeginArrowheadStyle()](#getbeginarrowheadstyle) | Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [getBeginArrowheadWidth()](#getbeginarrowheadwidth) | Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [getCapType()](#getcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [getCompoundType()](#getcompoundtype) | Specifies the line compound type. The value of the property is MsoLineStyle integer constant. |
| [getDashStyle()](#getdashstyle) | Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant. |
| [getEndArrowheadLength()](#getendarrowheadlength) | Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [getEndArrowheadStyle()](#getendarrowheadstyle) | Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [getEndArrowheadWidth()](#getendarrowheadwidth) | Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [getFillType()](#getfilltype) | Gets and sets fill type The value of the property is FillType integer constant. |
| [getGradientColor1()](#getgradientcolor1) | Returns the gradient color 1 for the specified fill. |
| [getGradientColor2()](#getgradientcolor2) | Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, t |
| [getGradientColorType()](#getgradientcolortype) | Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant. |
| [getGradientDegree()](#getgradientdegree) | Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) thr |
| [getGradientFill()](#getgradientfill) | Gets GradientFill object. |
| [getGradientStyle()](#getgradientstyle) | Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant. |
| [getGradientVariant()](#getgradientvariant) | Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4,  |
| [getImageData()](#getimagedata) | Gets and sets the picture image data. If the fill format is not custom texture format, returns null. |
| [getJoinType()](#getjointype) | Specifies the line join type. The value of the property is LineJoinType integer constant. |
| [getPattern()](#getpattern) | Represents an area's display pattern. The value of the property is FillPattern integer constant. |
| [getPatternFill()](#getpatternfill) | Gets PatternFill object. |
| [getPictureFormatType()](#getpictureformattype) | Gets and sets the picture format type. The value of the property is FillPictureType integer constant. |
| [getPresetColor()](#getpresetcolor) | Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer consta |
| [getScale()](#getscale) | Gets and sets the picture format scale. |
| [getSetType()](#getsettype) | Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obs |
| [getSolidFill()](#getsolidfill) | Gets SolidFill object. |
| [getTexture()](#gettexture) | Represents the texture type for the specified fill. The value of the property is TextureType integer constant. |
| [getTextureFill()](#gettexturefill) | Gets TextureFill object. |
| [getTransparency()](#gettransparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [getType()](#gettype) | Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete.  |
| [getWeight()](#getweight) | Gets or sets the weight of the line in unit of points. |
| [hashCode()](#hashcode) | Gets the hash code. |
| [setBeginArrowheadLength()](#setbeginarrowheadlength) | Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [setBeginArrowheadStyle()](#setbeginarrowheadstyle) | Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [setBeginArrowheadWidth()](#setbeginarrowheadwidth) | Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [setCapType()](#setcaptype) | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [setCompoundType()](#setcompoundtype) | Specifies the line compound type. The value of the property is MsoLineStyle integer constant. |
| [setDashStyle()](#setdashstyle) | Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant. |
| [setEndArrowheadLength()](#setendarrowheadlength) | Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [setEndArrowheadStyle()](#setendarrowheadstyle) | Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [setEndArrowheadWidth()](#setendarrowheadwidth) | Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [setFillType()](#setfilltype) | Gets and sets fill type The value of the property is FillType integer constant. |
| [setImageData()](#setimagedata) | Gets and sets the picture image data. If the fill format is not custom texture format, returns null. |
| [setJoinType()](#setjointype) | Specifies the line join type. The value of the property is LineJoinType integer constant. |
| [setOneColorGradient(color, degree, style, variant)](#setonecolorgradient) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setPattern()](#setpattern) | Represents an area's display pattern. The value of the property is FillPattern integer constant. |
| [setPictureFormatType()](#setpictureformattype) | Gets and sets the picture format type. The value of the property is FillPictureType integer constant. |
| [setPresetColorGradient(presetColor, style, variant)](#setpresetcolorgradient) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [setScale()](#setscale) | Gets and sets the picture format scale. |
| [setSetType()](#setsettype) | Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obs |
| [setTexture()](#settexture) | Represents the texture type for the specified fill. The value of the property is TextureType integer constant. |
| [setTransparency()](#settransparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [setTwoColorGradient(color1, color2, style, variant)](#settwocolorgradient) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(color1, transparency1, color2, transparency2, style, variant)](#settwocolorgradient-1) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setType()](#settype) | Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete.  |
| [setWeight()](#setweight) | Gets or sets the weight of the line in unit of points. |

### equals(obj) {#equals}

Determines whether this instance has the same value as another specified LineFormat object.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The |

**Returns:** boolean — `boolean` true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.

### getBeginArrowheadLength() {#getbeginarrowheadlength}

Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

### getBeginArrowheadStyle() {#getbeginarrowheadstyle}

Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

### getBeginArrowheadWidth() {#getbeginarrowheadwidth}

Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

### getCapType() {#getcaptype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

### getCompoundType() {#getcompoundtype}

Specifies the line compound type. The value of the property is MsoLineStyle integer constant.

### getDashStyle() {#getdashstyle}

Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant.

### getEndArrowheadLength() {#getendarrowheadlength}

Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

### getEndArrowheadStyle() {#getendarrowheadstyle}

Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

### getEndArrowheadWidth() {#getendarrowheadwidth}

Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

### getFillType() {#getfilltype}

Gets and sets fill type The value of the property is FillType integer constant.

### getGradientColor1() {#getgradientcolor1}

Returns the gradient color 1 for the specified fill.

### getGradientColor2() {#getgradientcolor2}

Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

### getGradientColorType() {#getgradientcolortype}

Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant.

### getGradientDegree() {#getgradientdegree}

Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) through 1.0 (light).

### getGradientFill() {#getgradientfill}

Gets GradientFill object.

### getGradientStyle() {#getgradientstyle}

Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant.

### getGradientVariant() {#getgradientvariant}

Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

### getImageData() {#getimagedata}

Gets and sets the picture image data. If the fill format is not custom texture format, returns null.

### getJoinType() {#getjointype}

Specifies the line join type. The value of the property is LineJoinType integer constant.

### getPattern() {#getpattern}

Represents an area's display pattern. The value of the property is FillPattern integer constant.

### getPatternFill() {#getpatternfill}

Gets PatternFill object.

### getPictureFormatType() {#getpictureformattype}

Gets and sets the picture format type. The value of the property is FillPictureType integer constant.

### getPresetColor() {#getpresetcolor}

Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer constant.

### getScale() {#getscale}

Gets and sets the picture format scale.

### getSetType() {#getsettype}

Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### getSolidFill() {#getsolidfill}

Gets SolidFill object.

### getTexture() {#gettexture}

Represents the texture type for the specified fill. The value of the property is TextureType integer constant.

### getTextureFill() {#gettexturefill}

Gets TextureFill object.

### getTransparency() {#gettransparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

### getType() {#gettype}

Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### getWeight() {#getweight}

Gets or sets the weight of the line in unit of points.

### hashCode() {#hashcode}

Gets the hash code.

**Returns:** Number — `Number`

### setBeginArrowheadLength() {#setbeginarrowheadlength}

Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

### setBeginArrowheadStyle() {#setbeginarrowheadstyle}

Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

### setBeginArrowheadWidth() {#setbeginarrowheadwidth}

Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

### setCapType() {#setcaptype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

### setCompoundType() {#setcompoundtype}

Specifies the line compound type. The value of the property is MsoLineStyle integer constant.

### setDashStyle() {#setdashstyle}

Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant.

### setEndArrowheadLength() {#setendarrowheadlength}

Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

### setEndArrowheadStyle() {#setendarrowheadstyle}

Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

### setEndArrowheadWidth() {#setendarrowheadwidth}

Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

### setFillType() {#setfilltype}

Gets and sets fill type The value of the property is FillType integer constant.

### setImageData() {#setimagedata}

Gets and sets the picture image data. If the fill format is not custom texture format, returns null.

### setJoinType() {#setjointype}

Specifies the line join type. The value of the property is LineJoinType integer constant.

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPattern() {#setpattern}

Represents an area's display pattern. The value of the property is FillPattern integer constant.

### setPictureFormatType() {#setpictureformattype}

Gets and sets the picture format type. The value of the property is FillPictureType integer constant.

### setPresetColorGradient(presetColor, style, variant) {#setpresetcolorgradient}

Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | Number | GradientPresetType |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setScale() {#setscale}

Gets and sets the picture format scale.

### setSetType() {#setsettype}

Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### setTexture() {#settexture}

Represents the texture type for the specified fill. The value of the property is TextureType integer constant.

### setTransparency() {#settransparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

### setTwoColorGradient(color1, color2, style, variant) {#settwocolorgradient}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(color1, transparency1, color2, transparency2, style, variant) {#settwocolorgradient-1}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | Number | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | Number | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setType() {#settype}

Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### setWeight() {#setweight}

Gets or sets the weight of the line in unit of points.
