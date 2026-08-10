---
title: "FontSetting Class"
linktitle: "FontSetting"
articleTitle: "FontSetting"
second_title: "Aspose.Cells for Python via Java"
description: "Represents a range of characters within the cell text."
type: docs
weight: 2480
url: /python-java/asposecells.api/fontsetting/
---

## FontSetting class

Represents a range of characters within the cell text.

## Constructors

| Name | Description |
| --- | --- |
| [FontSetting](#constructor) |  |

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Type](#type) | int | Gets the type of text node. The value of the property is TextNodeType integer constant. |
| [StartIndex](#startindex) | int | Gets the start index of the characters. |
| [Length](#length) | int | Gets the length of the characters. |
| [Font](#font) | Font | Returns the font of this object. |
| [TextOptions](#textoptions) | TextOptions | Returns the text options. |

## Methods

| Name | Description |
| --- | --- |
| [setWordArtStyle](#setwordartstyle) | Sets the preset WordArt style.

Only for the text of shape/chart. |

### FontSetting(startIndex, length, sheets) {#constructor}

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int |  |
| length | int |  |
| sheets | WorksheetCollection |  |

### FontSetting.Type property {#type}

Gets the type of text node. The value of the property is TextNodeType integer constant.

**Type:** int

### FontSetting.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** int

### FontSetting.Length property {#length}

Gets the length of the characters.

**Type:** int

### FontSetting.Font property {#font}

Returns the font of this object.

**Type:** Font

### FontSetting.TextOptions property {#textoptions}

Returns the text options.

**Type:** TextOptions

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style.

Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | int | A PresetWordArtStyle value. The preset WordArt style. |
