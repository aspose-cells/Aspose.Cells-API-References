---
title: "MsoFillFormat Class"
linktitle: "MsoFillFormat"
articleTitle: "MsoFillFormat"
second_title: "Aspose.Cells for Python via Java"
description: "Represents fill formatting for a shape."
type: docs
weight: 3730
url: /python-java/asposecells.api/msofillformat/
---

## MsoFillFormat class

Represents fill formatting for a shape.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [ForeColor](#forecolor) | Color | Gets and sets the fill fore color. |
| [Transparency](#transparency) | float | Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear). |
| [BackColor](#backcolor) | Color | Gets and sets the file back color. |
| [ImageData](#imagedata) | byte[] | Gets and sets the Texture and Picture fill data. |
| [Texture](#texture) | int | Gets the texture fill type. The value of the property is TextureType integer constant. |
| [IsVisible](#isvisible) | boolean | Indicates whether there is fill. |

## Methods

| Name | Description |
| --- | --- |
| [setOneColorGradient](#setonecolorgradient) | Sets the specified fill to a one-color gradient. |

### MsoFillFormat.ForeColor property {#forecolor}

Gets and sets the fill fore color.

**Type:** Color

### MsoFillFormat.Transparency property {#transparency}

Returns or sets the degree of transparency of the specified fill as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** float

### MsoFillFormat.BackColor property {#backcolor}

Gets and sets the file back color.

**Type:** Color

### MsoFillFormat.ImageData property {#imagedata}

Gets and sets the Texture and Picture fill data.

**Type:** byte[]

### MsoFillFormat.Texture property {#texture}

Gets the texture fill type. The value of the property is TextureType integer constant.

**Type:** int

### MsoFillFormat.IsVisible property {#isvisible}

Indicates whether there is fill.

**Type:** boolean

### setOneColorGradient(color, degree, style, variant) {#setonecolorgradient}

Sets the specified fill to a one-color gradient.

| Parameter | Type | Description |
| --- | --- | --- |
| color | Color | One gradient color. |
| degree | float | The gradient degree. Can be a value from 0.0 (dark) through 1.0 (light). |
| style | int | A GradientStyleType value. Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |
