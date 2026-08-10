---
title: "FontSettingCollection Class"
linktitle: "FontSettingCollection"
articleTitle: "FontSettingCollection"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the list of FontSetting ."
type: docs
weight: 2490
url: /python-java/asposecells.api/fontsettingcollection/
---

## FontSettingCollection class

Represents the list of FontSetting .

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [TextAlignment](#textalignment) | ShapeTextAlignment | Represents the alignment setting of the text body. |
| [TextParagraphs](#textparagraphs) | TextParagraphCollection | Gets all paragraphs. |
| [Text](#text) | String | Gets and sets the text of the shape. |
| [HtmlString](#htmlstring) | String | Gets and sets the html string which contains data and some formats in this shape. |
| [Count](#count) | int |  |
| [Item (int)](#itemint) | FontSetting | Gets the FontSetting by the index. |

## Methods

| Name | Description |
| --- | --- |
| [setWordArtStyle](#setwordartstyle) | Sets the preset WordArt style. |
| [getParagraphEnumerator](#getparagraphenumerator) | Gets the enumerator of the paragraphs. |
| [appendText](#appendtext) | Appends the text. |
| [insertText](#inserttext) | Insert index at the position. |
| [replace](#replace) | Replace the text. |
| [deleteText](#deletetext) | Delete some characters. |
| [format](#format) | Format the text with font setting. |
| [clear](#clear) | Clear all setting. |
| [equals](#equals) |  |
| [hashCode](#hashcode) |  |
| [removeAt](#removeat) |  |
| [iterator](#iterator) |  |
| [get](#get) | Reserved for internal use. |
| [contains](#contains) | Reserved for internal use. |
| [add](#add) | Reserved for internal use. |
| [indexOf](#indexof) | Reserved for internal use. |

### FontSettingCollection.TextAlignment property {#textalignment}

Represents the alignment setting of the text body.

**Type:** ShapeTextAlignment

### FontSettingCollection.TextParagraphs property {#textparagraphs}

Gets all paragraphs.

**Type:** TextParagraphCollection

### FontSettingCollection.Text property {#text}

Gets and sets the text of the shape.

**Type:** String

### FontSettingCollection.HtmlString property {#htmlstring}

Gets and sets the html string which contains data and some formats in this shape.

**Type:** String

### FontSettingCollection.Count property {#count}

**Type:** int

### FontSettingCollection.Item (int) property {#itemint}

Gets the FontSetting by the index.

**Type:** FontSetting

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style.

| Parameter | Type | Description |
| --- | --- | --- |
| style | int | A PresetWordArtStyle value. The preset WordArt style. |

### getParagraphEnumerator() {#getparagraphenumerator}

Gets the enumerator of the paragraphs.

### appendText(text) {#appendtext}

Appends the text.

| Parameter | Type | Description |
| --- | --- | --- |
| text | String | The text. |

### insertText(index, text) {#inserttext}

Insert index at the position.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| text | String | The text. |

### replace(index, count, text) (1 of 2) {#replace}

Replace the text.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| count | int | The count of characters. |
| text | String | The text. |

---

### replace(oldValue, newValue) (2 of 2) {#replace-1}

Replace the text.

| Parameter | Type | Description |
| --- | --- | --- |
| oldValue | String | The old text. |
| newValue | String | The new text. |

### deleteText(index, count) {#deletetext}

Delete some characters.

| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The start index. |
| count | int | The count of characters. |

### format(startIndex, length, font, flag) {#format}

Format the text with font setting.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | Font | The font. |
| flag | StyleFlag | The flags of the font. |

### clear() {#clear}

Clear all setting.

### equals(obj) {#equals}

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

### hashCode() {#hashcode}

### removeAt(index) {#removeat}

### iterator() {#iterator}

### get(index) {#get}

Reserved for internal use.

### contains(value) {#contains}

Reserved for internal use.

### add(value) {#add}

Reserved for internal use.

### indexOf(value) {#indexof}

Reserved for internal use.
