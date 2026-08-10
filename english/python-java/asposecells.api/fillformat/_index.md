---
title: "FillFormat Class"
linktitle: "FillFormat"
articleTitle: "FillFormat"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents fill formatting for a shape."
type: docs
weight: 2280
url: /python-java/asposecells.api/fillformat/
---

## FillFormat class

Encapsulates the object that represents fill formatting for a shape.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Type](#type) | int | Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete.  |
| [FillType](#filltype) | int | Gets and sets fill type The value of the property is FillType integer constant. |
| [Transparency](#transparency) | float | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetType](#settype) | int | Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obs |
| [GradientFill](#gradientfill) | GradientFill | Gets GradientFill object. |
| [TextureFill](#texturefill) | TextureFill | Gets TextureFill object. |
| [SolidFill](#solidfill) | SolidFill | Gets SolidFill object. |
| [PatternFill](#patternfill) | PatternFill | Gets PatternFill object. |
| [GradientColorType](#gradientcolortype) | int | Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant. |
| [GradientStyle](#gradientstyle) | int | Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant. |
| [GradientColor1](#gradientcolor1) | Color | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](#gradientcolor2) | Color | Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, t |
| [GradientDegree](#gradientdegree) | float | Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) thr |
| [GradientVariant](#gradientvariant) | int | Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4,  |
| [PresetColor](#presetcolor) | int | Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer consta |
| [Texture](#texture) | int | Represents the texture type for the specified fill. The value of the property is TextureType integer constant. |
| [Pattern](#pattern) | int | Represents an area's display pattern. The value of the property is FillPattern integer constant. |
| [PictureFormatType](#pictureformattype) | int | Gets and sets the picture format type. The value of the property is FillPictureType integer constant. |
| [Scale](#scale) | float | Gets and sets the picture format scale. |
| [ImageData](#imagedata) | byte[] | Gets and sets the picture image data. If the fill format is not custom texture format, returns null. |

## Methods

| Name | Description |
| --- | --- |
| [setOneColorGradient](#setonecolorgradient) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient](#settwocolorgradient) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setPresetColorGradient](#setpresetcolorgradient) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |
| [equals](#equals) |  |
| [hashCode](#hashcode) | Gets the hash code. |

### FillFormat.Type property {#type}

Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### FillFormat.FillType property {#filltype}

Gets and sets fill type The value of the property is FillType integer constant.

**Type:** int

### FillFormat.Transparency property {#transparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** float

### FillFormat.SetType property {#settype}

Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** int

### FillFormat.GradientFill property {#gradientfill}

Gets GradientFill object.

**Type:** GradientFill

### FillFormat.TextureFill property {#texturefill}

Gets TextureFill object.

**Type:** TextureFill

### FillFormat.SolidFill property {#solidfill}

Gets SolidFill object.

**Type:** SolidFill

### FillFormat.PatternFill property {#patternfill}

Gets PatternFill object.

**Type:** PatternFill

### FillFormat.GradientColorType property {#gradientcolortype}

Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant.

**Type:** int

### FillFormat.GradientStyle property {#gradientstyle}

Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant.

**Type:** int

### FillFormat.GradientColor1 property {#gradientcolor1}

Returns the gradient color 1 for the specified fill.

**Type:** Color

### FillFormat.GradientColor2 property {#gradientcolor2}

Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

**Type:** Color

### FillFormat.GradientDegree property {#gradientdegree}

Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) through 1.0 (light).

**Type:** float

### FillFormat.GradientVariant property {#gradientvariant}

Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

**Type:** int

### FillFormat.PresetColor property {#presetcolor}

Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer constant.

**Type:** int

### FillFormat.Texture property {#texture}

Represents the texture type for the specified fill. The value of the property is TextureType integer constant.

**Type:** int

### FillFormat.Pattern property {#pattern}

Represents an area's display pattern. The value of the property is FillPattern integer constant.

**Type:** int

### FillFormat.PictureFormatType property {#pictureformattype}

Gets and sets the picture format type. The value of the property is FillPictureType integer constant.

**Type:** int

### FillFormat.Scale property {#scale}

Gets and sets the picture format scale.

**Type:** float

### FillFormat.ImageData property {#imagedata}

Gets and sets the picture image data. If the fill format is not custom texture format, returns null.

**Type:** byte[]

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | float | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(color1, color2, style, variant) (1 of 2) {#settwocolorgradient}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

---

### setTwoColorGradient(color1, transparency1, color2, transparency2, style, variant) (2 of 2) {#settwocolorgradient-1}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | float | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | float | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPresetColorGradient(presetColor, style, variant) {#setpresetcolorgradient}

Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | int | A GradientPresetType value. Preset color type |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### equals(obj) {#equals}

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### hashCode() {#hashcode}

Gets the hash code.
