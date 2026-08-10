---
title: "TextParagraph Class"
linktitle: "TextParagraph"
articleTitle: "TextParagraph"
second_title: "Aspose.Cells for Python via Java"
description: "Represents the text paragraph setting."
type: docs
weight: 6750
url: /python-java/asposecells.api/textparagraph/
---

## TextParagraph class

Represents the text paragraph setting.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Bullet](#bullet) | Bullet | Gets the bullet. |
| [Type](#type) | int | Gets the type of text node. The value of the property is TextNodeType integer constant. |
| [LineSpaceSizeType](#linespacesizetype) | int | Gets and sets the amount of vertical white space that will be used within a paragraph. The value of the property is Line |
| [LineSpace](#linespace) | float | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [SpaceAfterSizeType](#spaceaftersizetype) | int | Gets and sets the amount of vertical white space that will be present after a paragraph. The value of the property is Li |
| [SpaceAfter](#spaceafter) | float | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [SpaceBeforeSizeType](#spacebeforesizetype) | int | Gets and sets the amount of vertical white space that will be present before a paragraph. The value of the property is L |
| [SpaceBefore](#spacebefore) | float | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [Stops](#stops) | TextTabStopCollection | Gets tab stop list. |
| [IsLatinLineBreak](#islatinlinebreak) | boolean | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [IsEastAsianLineBreak](#iseastasianlinebreak) | boolean | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [IsHangingPunctuation](#ishangingpunctuation) | boolean | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [RightMargin](#rightmargin) | float | Specifies the right margin of the paragraph. |
| [LeftMargin](#leftmargin) | float | Specifies the left margin of the paragraph. |
| [FirstLineIndent](#firstlineindent) | float | Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [FontAlignType](#fontaligntype) | int | Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the |
| [AlignmentType](#alignmenttype) | int | Gets and sets the text horizontal alignment type of the paragraph. The value of the property is TextAlignmentType intege |
| [DefaultTabSize](#defaulttabsize) | float | Gets and sets the default size for a tab character within this paragraph. |
| [Children](#children) | FontSetting[] | Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [StartIndex](#startindex) | int | Gets the start index of the characters. |
| [Length](#length) | int | Gets the length of the characters. |
| [Font](#font) | Font | Returns the font of this object. |
| [TextOptions](#textoptions) | TextOptions | Returns the text options. |

## Methods

| Name | Description |
| --- | --- |
| [setWordArtStyle](#setwordartstyle) | Sets the preset WordArt style.

Only for the text of shape/chart. |

### TextParagraph.Bullet property {#bullet}

Gets the bullet.

**Type:** Bullet

### TextParagraph.Type property {#type}

Gets the type of text node. The value of the property is TextNodeType integer constant.

**Type:** int

### TextParagraph.LineSpaceSizeType property {#linespacesizetype}

Gets and sets the amount of vertical white space that will be used within a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** int

### TextParagraph.LineSpace property {#linespace}

Gets and sets the amount of vertical white space that will be used within a paragraph.

**Type:** float

### TextParagraph.SpaceAfterSizeType property {#spaceaftersizetype}

Gets and sets the amount of vertical white space that will be present after a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** int

### TextParagraph.SpaceAfter property {#spaceafter}

Gets and sets the amount of vertical white space that will be present after a paragraph.

**Type:** float

### TextParagraph.SpaceBeforeSizeType property {#spacebeforesizetype}

Gets and sets the amount of vertical white space that will be present before a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** int

### TextParagraph.SpaceBefore property {#spacebefore}

Gets and sets the amount of vertical white space that will be present before a paragraph.

**Type:** float

### TextParagraph.Stops property {#stops}

Gets tab stop list.

**Type:** TextTabStopCollection

### TextParagraph.IsLatinLineBreak property {#islatinlinebreak}

Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added.

**Type:** boolean

### TextParagraph.IsEastAsianLineBreak property {#iseastasianlinebreak}

Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added.

**Type:** boolean

### TextParagraph.IsHangingPunctuation property {#ishangingpunctuation}

Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text.

**Type:** boolean

### TextParagraph.RightMargin property {#rightmargin}

Specifies the right margin of the paragraph.

**Type:** float

### TextParagraph.LeftMargin property {#leftmargin}

Specifies the left margin of the paragraph.

**Type:** float

### TextParagraph.FirstLineIndent property {#firstlineindent}

Specifies the indent size that will be applied to the first line of text in the paragraph.

**Type:** float

### TextParagraph.FontAlignType property {#fontaligntype}

Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. The value of the property is TextFontAlignType integer constant.

**Type:** int

### TextParagraph.AlignmentType property {#alignmenttype}

Gets and sets the text horizontal alignment type of the paragraph. The value of the property is TextAlignmentType integer constant.

**Type:** int

### TextParagraph.DefaultTabSize property {#defaulttabsize}

Gets and sets the default size for a tab character within this paragraph.

**Type:** float

### TextParagraph.Children property {#children}

Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.

**Type:** FontSetting[]

### TextParagraph.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** int

### TextParagraph.Length property {#length}

Gets the length of the characters.

**Type:** int

### TextParagraph.Font property {#font}

Returns the font of this object.

**Type:** Font

### TextParagraph.TextOptions property {#textoptions}

Returns the text options.

**Type:** TextOptions

### setWordArtStyle(style) {#setwordartstyle}

Sets the preset WordArt style.

Only for the text of shape/chart.

| Parameter | Type | Description |
| --- | --- | --- |
| style | int | A PresetWordArtStyle value. The preset WordArt style. |
