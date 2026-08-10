---
title: "FontSetting Class"
linktitle: "FontSetting"
articleTitle: "FontSetting"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents a range of characters within the cell text."
type: docs
weight: 2480
url: /php/aspose.cells/fontsetting/
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
| [Type](#type) | Number | Gets the type of text node. The value of the property is TextNodeType integer constant. |
| [StartIndex](#startindex) | Number | Gets the start index of the characters. |
| [Length](#length) | Number | Gets the length of the characters. |
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
| startIndex | Number |  |
| length | Number |  |
| sheets | WorksheetCollection |  |

### FontSetting.Type property {#type}

Gets the type of text node. The value of the property is TextNodeType integer constant.

**Type:** Number

### FontSetting.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** Number

### FontSetting.Length property {#length}

Gets the length of the characters.

**Type:** Number

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
| style | Number | A PresetWordArtStyle value. The preset WordArt style. |
