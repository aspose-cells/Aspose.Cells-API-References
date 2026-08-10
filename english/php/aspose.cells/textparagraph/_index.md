---
title: "TextParagraph Class"
linktitle: "TextParagraph"
articleTitle: "TextParagraph"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the text paragraph setting."
type: docs
weight: 6750
url: /php/aspose.cells/textparagraph/
---

## TextParagraph class

Represents the text paragraph setting.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Bullet](#bullet) | Bullet | Gets the bullet. |
| [Type](#type) | Number | Gets the type of text node. The value of the property is TextNodeType integer constant. |
| [LineSpaceSizeType](#linespacesizetype) | Number | Gets and sets the amount of vertical white space that will be used within a paragraph. The value of the property is Line |
| [LineSpace](#linespace) | Number | Gets and sets the amount of vertical white space that will be used within a paragraph. |
| [SpaceAfterSizeType](#spaceaftersizetype) | Number | Gets and sets the amount of vertical white space that will be present after a paragraph. The value of the property is Li |
| [SpaceAfter](#spaceafter) | Number | Gets and sets the amount of vertical white space that will be present after a paragraph. |
| [SpaceBeforeSizeType](#spacebeforesizetype) | Number | Gets and sets the amount of vertical white space that will be present before a paragraph. The value of the property is L |
| [SpaceBefore](#spacebefore) | Number | Gets and sets the amount of vertical white space that will be present before a paragraph. |
| [Stops](#stops) | TextTabStopCollection | Gets tab stop list. |
| [IsLatinLineBreak](#islatinlinebreak) | boolean | Specifies whether a Latin word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [IsEastAsianLineBreak](#iseastasianlinebreak) | boolean | Specifies whether an East Asian word can be broken in half and wrapped onto the next line without a hyphen being added. |
| [IsHangingPunctuation](#ishangingpunctuation) | boolean | Specifies whether punctuation is to be forcefully laid out on a line of text or put on a different line of text. |
| [RightMargin](#rightmargin) | Number | Specifies the right margin of the paragraph. |
| [LeftMargin](#leftmargin) | Number | Specifies the left margin of the paragraph. |
| [FirstLineIndent](#firstlineindent) | Number | Specifies the indent size that will be applied to the first line of text in the paragraph. |
| [FontAlignType](#fontaligntype) | Number | Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the |
| [AlignmentType](#alignmenttype) | Number | Gets and sets the text horizontal alignment type of the paragraph. The value of the property is TextAlignmentType intege |
| [DefaultTabSize](#defaulttabsize) | Number | Gets and sets the default size for a tab character within this paragraph. |
| [Children](#children) | FontSetting[] | Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself. |
| [StartIndex](#startindex) | Number | Gets the start index of the characters. |
| [Length](#length) | Number | Gets the length of the characters. |
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

**Type:** Number

### TextParagraph.LineSpaceSizeType property {#linespacesizetype}

Gets and sets the amount of vertical white space that will be used within a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** Number

### TextParagraph.LineSpace property {#linespace}

Gets and sets the amount of vertical white space that will be used within a paragraph.

**Type:** Number

### TextParagraph.SpaceAfterSizeType property {#spaceaftersizetype}

Gets and sets the amount of vertical white space that will be present after a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** Number

### TextParagraph.SpaceAfter property {#spaceafter}

Gets and sets the amount of vertical white space that will be present after a paragraph.

**Type:** Number

### TextParagraph.SpaceBeforeSizeType property {#spacebeforesizetype}

Gets and sets the amount of vertical white space that will be present before a paragraph. The value of the property is LineSpaceSizeType integer constant.

**Type:** Number

### TextParagraph.SpaceBefore property {#spacebefore}

Gets and sets the amount of vertical white space that will be present before a paragraph.

**Type:** Number

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

**Type:** Number

### TextParagraph.LeftMargin property {#leftmargin}

Specifies the left margin of the paragraph.

**Type:** Number

### TextParagraph.FirstLineIndent property {#firstlineindent}

Specifies the indent size that will be applied to the first line of text in the paragraph.

**Type:** Number

### TextParagraph.FontAlignType property {#fontaligntype}

Determines where vertically on a line of text the actual words are positioned. This deals with vertical placement of the characters with respect to the baselines. The value of the property is TextFontAlignType integer constant.

**Type:** Number

### TextParagraph.AlignmentType property {#alignmenttype}

Gets and sets the text horizontal alignment type of the paragraph. The value of the property is TextAlignmentType integer constant.

**Type:** Number

### TextParagraph.DefaultTabSize property {#defaulttabsize}

Gets and sets the default size for a tab character within this paragraph.

**Type:** Number

### TextParagraph.Children property {#children}

Gets all text runs in this paragraph. If this paragraph is empty, return paragraph itself.

**Type:** FontSetting[]

### TextParagraph.StartIndex property {#startindex}

Gets the start index of the characters.

**Type:** Number

### TextParagraph.Length property {#length}

Gets the length of the characters.

**Type:** Number

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
| style | Number | A PresetWordArtStyle value. The preset WordArt style. |
