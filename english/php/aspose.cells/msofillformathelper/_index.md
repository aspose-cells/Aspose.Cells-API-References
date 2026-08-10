---
title: "MsoFillFormatHelper Class"
linktitle: "MsoFillFormatHelper"
articleTitle: "MsoFillFormatHelper"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents fill formatting for a shape."
type: docs
weight: 3740
url: /php/aspose.cells/msofillformathelper/
---

## MsoFillFormatHelper class

Represents fill formatting for a shape.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ForeColor](#forecolor) | Color | Gets and sets the fill fore color. |
| [ForeColorTransparency](#forecolortransparency) | Number | Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [BackColor](#backcolor) | Color | Gets and sets the file back color. |
| [ImageData](#imagedata) | byte[] | Gets and sets the Texture and Picture fill data. |
| [Texture](#texture) | Number | Gets the texture fill type. The value of the property is TextureType integer constant. |
| [IsVisible](#isvisible) | boolean | Indicates whether there is fill. |

## Methods

| Name | Description |
| --- | --- |
| [setOneColorGradient](#setonecolorgradient) | Sets the specified fill to a one-color gradient. |

### MsoFillFormatHelper.ForeColor property {#forecolor}

Gets and sets the fill fore color.

**Type:** Color

### MsoFillFormatHelper.ForeColorTransparency property {#forecolortransparency}

Returns or sets the degree of fore color of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** Number

### MsoFillFormatHelper.BackColor property {#backcolor}

Gets and sets the file back color.

**Type:** Color

### MsoFillFormatHelper.ImageData property {#imagedata}

Gets and sets the Texture and Picture fill data.

**Type:** byte[]

### MsoFillFormatHelper.Texture property {#texture}

Gets the texture fill type. The value of the property is TextureType integer constant.

**Type:** Number

### MsoFillFormatHelper.IsVisible property {#isvisible}

Indicates whether there is fill.

**Type:** boolean

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | Number | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | Number | A GradientStyleType value. Gradient shading style. |
| variant | Number | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
