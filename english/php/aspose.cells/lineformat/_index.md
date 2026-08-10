---
title: "LineFormat Class"
linktitle: "LineFormat"
articleTitle: "LineFormat"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents all setting of the line."
type: docs
weight: 3350
url: /php/aspose.cells/lineformat/
---

## LineFormat class

Represents all setting of the line.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CompoundType](#compoundtype) | Number | Specifies the line compound type. The value of the property is MsoLineStyle integer constant. |
| [DashStyle](#dashstyle) | Number | Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant. |
| [CapType](#captype) | Number | Specifies the ending caps. The value of the property is LineCapType integer constant. |
| [JoinType](#jointype) | Number | Specifies the line join type. The value of the property is LineJoinType integer constant. |
| [BeginArrowheadStyle](#beginarrowheadstyle) | Number | Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [BeginArrowheadWidth](#beginarrowheadwidth) | Number | Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [BeginArrowheadLength](#beginarrowheadlength) | Number | Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [EndArrowheadStyle](#endarrowheadstyle) | Number | Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant. |
| [EndArrowheadWidth](#endarrowheadwidth) | Number | Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant. |
| [EndArrowheadLength](#endarrowheadlength) | Number | Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant. |
| [Weight](#weight) | Number | Gets or sets the weight of the line in unit of points. |
| [Type](#type) | Number | Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete.  |
| [FillType](#filltype) | Number | Gets and sets fill type The value of the property is FillType integer constant. |
| [Transparency](#transparency) | Number | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [SetType](#settype) | Number | Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obs |
| [GradientFill](#gradientfill) | GradientFill | Gets GradientFill object. |
| [TextureFill](#texturefill) | TextureFill | Gets TextureFill object. |
| [SolidFill](#solidfill) | SolidFill | Gets SolidFill object. |
| [PatternFill](#patternfill) | PatternFill | Gets PatternFill object. |
| [GradientColorType](#gradientcolortype) | Number | Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant. |
| [GradientStyle](#gradientstyle) | Number | Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant. |
| [GradientColor1](#gradientcolor1) | Color | Returns the gradient color 1 for the specified fill. |
| [GradientColor2](#gradientcolor2) | Color | Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, t |
| [GradientDegree](#gradientdegree) | Number | Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) thr |
| [GradientVariant](#gradientvariant) | Number | Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4,  |
| [PresetColor](#presetcolor) | Number | Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer consta |
| [Texture](#texture) | Number | Represents the texture type for the specified fill. The value of the property is TextureType integer constant. |
| [Pattern](#pattern) | Number | Represents an area's display pattern. The value of the property is FillPattern integer constant. |
| [PictureFormatType](#pictureformattype) | Number | Gets and sets the picture format type. The value of the property is FillPictureType integer constant. |
| [Scale](#scale) | Number | Gets and sets the picture format scale. |
| [ImageData](#imagedata) | byte[] | Gets and sets the picture image data. If the fill format is not custom texture format, returns null. |

## Methods

| Name | Description |
| --- | --- |
| [hashCode](#hashcode) | Gets the hash code. |
| [equals](#equals) | Determines whether this instance has the same value as another specified LineFormat object. |
| [setOneColorGradient](#setonecolorgradient) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient](#settwocolorgradient) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setPresetColorGradient](#setpresetcolorgradient) | Sets the specified fill to a preset-color gradient. Only applies for Excel 2007. |

### LineFormat.CompoundType property {#compoundtype}

Specifies the line compound type. The value of the property is MsoLineStyle integer constant.

**Type:** Number

### LineFormat.DashStyle property {#dashstyle}

Specifies the line dash type. The value of the property is MsoLineDashStyle integer constant.

**Type:** Number

### LineFormat.CapType property {#captype}

Specifies the ending caps. The value of the property is LineCapType integer constant.

**Type:** Number

### LineFormat.JoinType property {#jointype}

Specifies the line join type. The value of the property is LineJoinType integer constant.

**Type:** Number

### LineFormat.BeginArrowheadStyle property {#beginarrowheadstyle}

Gets and sets the begin arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

**Type:** Number

### LineFormat.BeginArrowheadWidth property {#beginarrowheadwidth}

Gets and sets the begin arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

**Type:** Number

### LineFormat.BeginArrowheadLength property {#beginarrowheadlength}

Gets and sets the begin arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

**Type:** Number

### LineFormat.EndArrowheadStyle property {#endarrowheadstyle}

Gets and sets the end arrow type of the line. The value of the property is MsoArrowheadStyle integer constant.

**Type:** Number

### LineFormat.EndArrowheadWidth property {#endarrowheadwidth}

Gets and sets the end arrow width type of the line. The value of the property is MsoArrowheadWidth integer constant.

**Type:** Number

### LineFormat.EndArrowheadLength property {#endarrowheadlength}

Gets and sets the end arrow length type of the line. The value of the property is MsoArrowheadLength integer constant.

**Type:** Number

### LineFormat.Weight property {#weight}

Gets or sets the weight of the line in unit of points.

**Type:** Number

### LineFormat.Type property {#type}

Gets and sets the fill type. The value of the property is FillType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### LineFormat.FillType property {#filltype}

Gets and sets fill type The value of the property is FillType integer constant.

**Type:** Number

### LineFormat.Transparency property {#transparency}

Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** Number

### LineFormat.SetType property {#settype}

Gets the fill format set type. The value of the property is FormatSetType integer constant. NOTE: This member is now obsolete. Instead, please use FillFormat.FillType property instead. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Type:** Number

### LineFormat.GradientFill property {#gradientfill}

Gets GradientFill object.

**Type:** GradientFill

### LineFormat.TextureFill property {#texturefill}

Gets TextureFill object.

**Type:** TextureFill

### LineFormat.SolidFill property {#solidfill}

Gets SolidFill object.

**Type:** SolidFill

### LineFormat.PatternFill property {#patternfill}

Gets PatternFill object.

**Type:** PatternFill

### LineFormat.GradientColorType property {#gradientcolortype}

Returns the gradient color type for the specified fill. The value of the property is GradientColorType integer constant.

**Type:** Number

### LineFormat.GradientStyle property {#gradientstyle}

Returns the gradient style for the specified fill. The value of the property is GradientStyleType integer constant.

**Type:** Number

### LineFormat.GradientColor1 property {#gradientcolor1}

Returns the gradient color 1 for the specified fill.

**Type:** Color

### LineFormat.GradientColor2 property {#gradientcolor2}

Returns the gradient color 2 for the specified fill. Only when the gradient color type is GradientColorType.TwoColors, this property is meaningful.

**Type:** Color

### LineFormat.GradientDegree property {#gradientdegree}

Returns the gradient degree for the specified fill. Only applies for Excel 2007. Can only be a value from 0.0 (dark) through 1.0 (light).

**Type:** Number

### LineFormat.GradientVariant property {#gradientvariant}

Returns the gradient variant for the specified fill. Only applies for Excel 2007. Can only be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2.

**Type:** Number

### LineFormat.PresetColor property {#presetcolor}

Returns the gradient preset color for the specified fill. The value of the property is GradientPresetType integer constant.

**Type:** Number

### LineFormat.Texture property {#texture}

Represents the texture type for the specified fill. The value of the property is TextureType integer constant.

**Type:** Number

### LineFormat.Pattern property {#pattern}

Represents an area's display pattern. The value of the property is FillPattern integer constant.

**Type:** Number

### LineFormat.PictureFormatType property {#pictureformattype}

Gets and sets the picture format type. The value of the property is FillPictureType integer constant.

**Type:** Number

### LineFormat.Scale property {#scale}

Gets and sets the picture format scale.

**Type:** Number

### LineFormat.ImageData property {#imagedata}

Gets and sets the picture image data. If the fill format is not custom texture format, returns null.

**Type:** byte[]

### hashCode() {#hashcode}

Gets the hash code.

### equals(obj) {#equals}

Determines whether this instance has the same value as another specified LineFormat object.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object | The LineFormat object to compare with this instance. |

**Returns:** true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setTwoColorGradient(color1, color2, style, variant) (1 of 2) {#settwocolorgradient}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| color2 | Color | Two gradient color. |
| style | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

---

### setTwoColorGradient(color1, transparency1, color2, transparency2, style, variant) (2 of 2) {#settwocolorgradient-1}

Sets the specified fill to a two-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color1 | Color | One gradient color. |
| transparency1 | Number | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | Color | Two gradient color. |
| transparency2 | Number | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPresetColorGradient(presetColor, style, variant) {#setpresetcolorgradient}

Sets the specified fill to a preset-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | Number | A GradientPresetType value. Preset color type |
| style | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
