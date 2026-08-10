---
title: "GradientFill"
linktitle: "GradientFill"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the gradient fill."
type: docs
weight: 1690
url: /nodejs/aspose.cells/gradientfill/
---

## GradientFill class

Represents the gradient fill.

## Methods

| Name | Description |
| --- | --- |
| [equals(obj)](#equals) | / |
| [getAngle()](#getangle) | The angle of linear fill. |
| [getDirectionType()](#getdirectiontype) | Gets the gradient direction type. The value of the property is GradientDirectionType integer constant. |
| [getFillType()](#getfilltype) | Gets the gradient fill type. The value of the property is GradientFillType integer constant. |
| [getGradientColor1()](#getgradientcolor1) | Gets gradient color 1. Applies to Excel97-2003 |
| [getGradientColor2()](#getgradientcolor2) | Gets gradient color 2. Applies to Excel97-2003 |
| [getGradientColorType()](#getgradientcolortype) | Gets gradient color type. Applies to Excel97-2003 The value of the property is GradientColorType integer constant. |
| [getGradientDegree()](#getgradientdegree) | Gets gradient degree. Applies to Excel97-2003 |
| [getGradientStops()](#getgradientstops) | Represents the gradient stop collection. |
| [getGradientStyle()](#getgradientstyle) | Gets gradient style type. Applies to Excel97-2003 The value of the property is GradientStyleType integer constant. |
| [getPresetColor()](#getpresetcolor) | Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientP |
| [getVariant()](#getvariant) | Gets variant. Applies to Excel97-2003 |
| [hashCode()](#hashcode) | Gets the hash code. |
| [setAngle()](#setangle) | The angle of linear fill. |
| [setGradient(type, angle, direction)](#setgradient) | Set the gradient fill type and direction. |
| [setOneColorGradient(color, degree, style, variant)](#setonecolorgradient) | Sets the specified fill to a one-color gradient. Only applies for Excel 2007. |
| [setPresetColor()](#setpresetcolor) | Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientP |
| [setPresetColorGradient(presetColor, style, variant)](#setpresetcolorgradient) | Sets the specified fill to a preset-color gradient. Only applies for Excel 97-2003 |
| [setPresetThemeGradient(gradientType, themeColorType)](#setpresetthemegradient) | Sets preset theme gradient fill. |
| [setTwoColorGradient(color1, color2, style, variant)](#settwocolorgradient) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |
| [setTwoColorGradient(color1, transparency1, color2, transparency2, style, variant)](#settwocolorgradient-1) | Sets the specified fill to a two-color gradient. Only applies for Excel 2007. |

### equals(obj) {#equals}

/

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

**Returns:** boolean — `boolean`

### getAngle() {#getangle}

The angle of linear fill.

### getDirectionType() {#getdirectiontype}

Gets the gradient direction type. The value of the property is GradientDirectionType integer constant.

### getFillType() {#getfilltype}

Gets the gradient fill type. The value of the property is GradientFillType integer constant.

### getGradientColor1() {#getgradientcolor1}

Gets gradient color 1. Applies to Excel97-2003

### getGradientColor2() {#getgradientcolor2}

Gets gradient color 2. Applies to Excel97-2003

### getGradientColorType() {#getgradientcolortype}

Gets gradient color type. Applies to Excel97-2003 The value of the property is GradientColorType integer constant.

### getGradientDegree() {#getgradientdegree}

Gets gradient degree. Applies to Excel97-2003

### getGradientStops() {#getgradientstops}

Represents the gradient stop collection.

### getGradientStyle() {#getgradientstyle}

Gets gradient style type. Applies to Excel97-2003 The value of the property is GradientStyleType integer constant.

### getPresetColor() {#getpresetcolor}

Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientPresetType integer constant.

### getVariant() {#getvariant}

Gets variant. Applies to Excel97-2003

### hashCode() {#hashcode}

Gets the hash code.

**Returns:** Number — `Number`

### setAngle() {#setangle}

The angle of linear fill.

### setGradient(type, angle, direction) {#setgradient}

Set the gradient fill type and direction.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | GradientFillType |
| angle | Number | The angle. Only applies for GradientFillType.Linear. |
| direction | Number | GradientDirectionType |

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient. Only applies for Excel 2007.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPresetColor() {#setpresetcolor}

Returns the gradient preset color for the specified fill. Applies to Excel97-2003 The value of the property is GradientPresetType integer constant.

### setPresetColorGradient(presetColor, style, variant) {#setpresetcolorgradient}

Sets the specified fill to a preset-color gradient. Only applies for Excel 97-2003

| Parameter | Type | Description |
| --- | --- | --- |
| presetColor | Number | GradientPresetType |
| style | Number | GradientStyleType |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |

### setPresetThemeGradient(gradientType, themeColorType) {#setpresetthemegradient}

Sets preset theme gradient fill.

| Parameter | Type | Description |
| --- | --- | --- |
| gradientType | Number | PresetThemeGradientType |
| themeColorType | Number | ThemeColorType |

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
