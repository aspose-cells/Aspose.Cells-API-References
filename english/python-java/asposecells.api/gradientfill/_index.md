---
title: "GradientFill Class"
linktitle: "GradientFill"
articleTitle: "GradientFill"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the gradient fill."
type: docs
weight: 2690
url: /python-java/asposecells.api/gradientfill/
---

## GradientFill class

Represents the gradient fill.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [GradientStops](#gradientstops) | GradientStopCollection | Represents the gradient stop collection. |
| [FillType](#filltype) | int | Gets the gradient fill type. The value of the property is GradientFillType integer constant. |
| [DirectionType](#directiontype) | int | Gets the gradient direction type. The value of the property is GradientDirectionType integer constant. |
| [Angle](#angle) | float | The angle of linear fill. |
| [GradientColor1](#gradientcolor1) | Color | Gets gradient color 1. Applies to Excel97-2003 |
| [GradientColor2](#gradientcolor2) | Color | Gets gradient color 2. Applies to Excel97-2003 |
| [GradientDegree](#gradientdegree) | float | Gets gradient degree. Applies to Excel97-2003 |
| [GradientColorType](#gradientcolortype) | int | Gets gradient color type. Applies to Excel97-2003 The value of the property is GradientColorType integer constant. |
| [PresetColor](#presetcolor) | int | Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientP |
| [Variant](#variant) | int | Gets variant. Applies to Excel97-2003 |
| [GradientStyle](#gradientstyle) | int | Gets gradient style type. Applies to Excel97-2003 The value of the property is GradientStyleType integer constant. |

## Methods

| Name | Description |
| --- | --- |
| [setGradient](#setgradient) | Set the gradient fill type and direction. |
| [setPresetThemeGradient](#setpresetthemegradient) | Sets preset theme gradient fill. |
| [setPresetColorGradient](#setpresetcolorgradient) | Sets the specified fill to a preset-color gradient. Only applies for Excel 97-2003 |
| [setOneColorGradient](#setonecolorgradient) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient](#settwocolorgradient) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [equals](#equals) | / |
| [hashCode](#hashcode) | Gets the hash code. |

### GradientFill.GradientStops property {#gradientstops}

Represents the gradient stop collection.

**Type:** GradientStopCollection

### GradientFill.FillType property {#filltype}

Gets the gradient fill type. The value of the property is GradientFillType integer constant.

**Type:** int

### GradientFill.DirectionType property {#directiontype}

Gets the gradient direction type. The value of the property is GradientDirectionType integer constant.

**Type:** int

### GradientFill.Angle property {#angle}

The angle of linear fill.

**Type:** float

### GradientFill.GradientColor1 property {#gradientcolor1}

Gets gradient color 1. Applies to Excel97-2003

**Type:** Color

### GradientFill.GradientColor2 property {#gradientcolor2}

Gets gradient color 2. Applies to Excel97-2003

**Type:** Color

### GradientFill.GradientDegree property {#gradientdegree}

Gets gradient degree. Applies to Excel97-2003

**Type:** float

### GradientFill.GradientColorType property {#gradientcolortype}

Gets gradient color type. Applies to Excel97-2003 The value of the property is GradientColorType integer constant.

**Type:** int

### GradientFill.PresetColor property {#presetcolor}

Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientPresetType integer constant.

**Type:** int

### GradientFill.Variant property {#variant}

Gets variant. Applies to Excel97-2003

**Type:** int

### GradientFill.GradientStyle property {#gradientstyle}

Gets gradient style type. Applies to Excel97-2003 The value of the property is GradientStyleType integer constant.

**Type:** int

### setGradient(type, angle, direction) {#setgradient}

Set the gradient fill type and direction.

| Parameter | Type | Description |
| --- | --- | --- |
| type | int | A GradientFillType value. Gradient fill type. |
| angle | float | The angle. Only applies for GradientFillType.Linear. |
| direction | int | A GradientDirectionType value. The direction type. Only applies for GradientFillType.Radial and GradientFillType.Rectangle. |

### setPresetThemeGradient(gradientType, themeColorType) {#setpresetthemegradient}

Sets preset theme gradient fill.

| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | int | A PresetThemeGradientType value. The preset gradient type. |
| themeColorType | int | A ThemeColorType value. The theme color type. |

### setPresetColorGradient(presetColor, style, variant) {#setpresetcolorgradient}

Sets the specified fill to a preset-color gradient. Only applies for Excel 97-2003

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | int | A GradientPresetType value. Preset color type |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

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

### equals(obj) {#equals}

/

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### hashCode() {#hashcode}

Gets the hash code.
