---
title: "Comment Class"
linktitle: "Comment"
articleTitle: "Comment"
second_title: "Aspose.Cells for Python via Java"
description: "Encapsulates the object that represents a cell comment."
type: docs
weight: 1050
url: /python-java/asposecells.api/comment/
---

## Comment class

Encapsulates the object that represents a cell comment.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [Author](#author) | String | Gets and sets Name of the original comment author |
| [CommentShape](#commentshape) | CommentShape | Get a Shape object that represents the shape attached to the specified comment. |
| [Row](#row) | int | Gets the row index of the comment. |
| [Column](#column) | int | Gets the column index of the comment. |
| [IsThreadedComment](#isthreadedcomment) | boolean | Indicates whether this comment is a threaded comment. |
| [ThreadedComments](#threadedcomments) | ThreadedCommentCollection | Gets the list of threaded comments; |
| [Note](#note) | String | Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel coul |
| [HtmlNote](#htmlnote) | String | Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the n |
| [Font](#font) | Font | Gets the font of comment. |
| [IsVisible](#isvisible) | boolean | Represents if the comment is visible or not. |
| [TextOrientationType](#textorientationtype) | int | Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constan |
| [TextHorizontalAlignment](#texthorizontalalignment) | int | Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer  |
| [TextVerticalAlignment](#textverticalalignment) | int | Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer co |
| [AutoSize](#autosize) | boolean | Indicates if size of comment is adjusted automatically according to its content. |
| [HeightCM](#heightcm) | float | Represents the height of the comment, in unit of centimeters. |
| [WidthCM](#widthcm) | float | Represents the width of the comment, in unit of centimeters. |
| [Width](#width) | int | Represents the width of the comment, in unit of pixels. |
| [Height](#height) | int | Represents the Height of the comment, in unit of pixels. |
| [WidthInch](#widthinch) | float | Represents the width of the comment, in unit of inches. |
| [HeightInch](#heightinch) | float | Represents the height of the comment, in unit of inches. |

## Methods

| Name | Description |
| --- | --- |
| [formatCharacters](#formatcharacters) | Format some characters with the font setting. |
| [characters](#characters) | Returns a Characters object that represents a range of characters within the comment text. |
| [getRichFormattings](#getrichformattings) | Returns all Characters objects that represents a range of characters within the comment text. |

### Comment.Author property {#author}

Gets and sets Name of the original comment author

**Type:** String

### Comment.CommentShape property {#commentshape}

Get a Shape object that represents the shape attached to the specified comment.

**Type:** CommentShape

### Comment.Row property {#row}

Gets the row index of the comment.

**Type:** int

### Comment.Column property {#column}

Gets the column index of the comment.

**Type:** int

### Comment.IsThreadedComment property {#isthreadedcomment}

Indicates whether this comment is a threaded comment.

**Type:** boolean

### Comment.ThreadedComments property {#threadedcomments}

Gets the list of threaded comments;

**Type:** ThreadedCommentCollection

### Comment.Note property {#note}

Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

**Type:** String

### Comment.HtmlNote property {#htmlnote}

Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

**Type:** String

### Comment.Font property {#font}

Gets the font of comment.

**Type:** Font

### Comment.IsVisible property {#isvisible}

Represents if the comment is visible or not.

**Type:** boolean

### Comment.TextOrientationType property {#textorientationtype}

Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constant.

**Type:** int

### Comment.TextHorizontalAlignment property {#texthorizontalalignment}

Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer constant.

**Type:** int

### Comment.TextVerticalAlignment property {#textverticalalignment}

Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer constant.

**Type:** int

### Comment.AutoSize property {#autosize}

Indicates if size of comment is adjusted automatically according to its content.

**Type:** boolean

### Comment.HeightCM property {#heightcm}

Represents the height of the comment, in unit of centimeters.

**Type:** float

### Comment.WidthCM property {#widthcm}

Represents the width of the comment, in unit of centimeters.

**Type:** float

### Comment.Width property {#width}

Represents the width of the comment, in unit of pixels.

**Type:** int

### Comment.Height property {#height}

Represents the Height of the comment, in unit of pixels.

**Type:** int

### Comment.WidthInch property {#widthinch}

Represents the width of the comment, in unit of inches.

**Type:** float

### Comment.HeightInch property {#heightinch}

Represents the height of the comment, in unit of inches.

**Type:** float

### formatCharacters(startIndex, length, font, flag) {#formatcharacters}

Format some characters with the font setting.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the comment text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:** Characters object.

### getRichFormattings() {#getrichformattings}

Returns all Characters objects that represents a range of characters within the comment text.

**Returns:** All Characters objects
