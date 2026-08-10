---
title: "CellsColor Class"
linktitle: "CellsColor"
articleTitle: "CellsColor"
second_title: "Aspose.Cells for Python via Java"
description: "Represents all types of color."
type: docs
weight: 630
url: /python-java/asposecells.api/cellscolor/
---

## CellsColor class

Represents all types of color.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [IsShapeColor](#isshapecolor) | boolean | Gets and set the color which should apply to cell or shape. The expression of the color of the cell and the shape is dif |
| [Type](#type) | int | The color type. The value of the property is ColorType integer constant. |
| [ThemeColor](#themecolor) | ThemeColor | Gets the theme color. Only applies for theme color type. |
| [ColorIndex](#colorindex) | int | Gets and sets the color index in the color palette. Only applies of indexed color. |
| [Color](#color) | Color | Gets and sets the RGB color. |
| [Argb](#argb) | int | Gets and sets the color from a 32-bit ARGB value. |
| [Transparency](#transparency) | float | Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear). |

## Methods

| Name | Description |
| --- | --- |
| [setTintOfShapeColor](#settintofshapecolor) | Set the tint of the shape color |

### CellsColor.IsShapeColor property {#isshapecolor}

Gets and set the color which should apply to cell or shape. The expression of the color of the cell and the shape is different. For example: the theme color with same tint value will be not same in the cell and the shape.

**Type:** boolean

### CellsColor.Type property {#type}

The color type. The value of the property is ColorType integer constant.

**Type:** int

### CellsColor.ThemeColor property {#themecolor}

Gets the theme color. Only applies for theme color type.

**Type:** ThemeColor

### CellsColor.ColorIndex property {#colorindex}

Gets and sets the color index in the color palette. Only applies of indexed color.

**Type:** int

### CellsColor.Color property {#color}

Gets and sets the RGB color.

**Type:** Color

### CellsColor.Argb property {#argb}

Gets and sets the color from a 32-bit ARGB value.

**Type:** int

### CellsColor.Transparency property {#transparency}

Gets and sets transparency as a value from 0.0 (opaque) through 1.0 (clear).

**Type:** float

### setTintOfShapeColor(tint) {#settintofshapecolor}

Set the tint of the shape color

| Parameter | Type | Description |
| --- | --- | --- |
| tint | float |  |
