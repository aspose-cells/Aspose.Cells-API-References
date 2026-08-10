---
title: "Comment"
linktitle: "Comment"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Encapsulates the object that represents a cell comment."
type: docs
weight: 730
url: /nodejs/aspose.cells/comment/
---

## Comment class

Encapsulates the object that represents a cell comment.

## Methods

| Name | Description |
| --- | --- |
| [characters(startIndex, length)](#characters) | Returns a Characters object that represents a range of characters within the comment text. |
| [formatCharacters(startIndex, length, font, flag)](#formatcharacters) | Format some characters with the font setting. |
| [getAuthor()](#getauthor) | Gets and sets Name of the original comment author |
| [getAutoSize()](#getautosize) | Indicates if size of comment is adjusted automatically according to its content. |
| [getColumn()](#getcolumn) | Gets the column index of the comment. |
| [getCommentShape()](#getcommentshape) | Get a Shape object that represents the shape attached to the specified comment. |
| [getFont()](#getfont) | Gets the font of comment. |
| [getHeight()](#getheight) | Represents the Height of the comment, in unit of pixels. |
| [getHeightCM()](#getheightcm) | Represents the height of the comment, in unit of centimeters. |
| [getHeightInch()](#getheightinch) | Represents the height of the comment, in unit of inches. |
| [getHtmlNote()](#gethtmlnote) | Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the n |
| [getNote()](#getnote) | Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel coul |
| [getRichFormattings()](#getrichformattings) | Returns all Characters objects that represents a range of characters within the comment text. |
| [getRow()](#getrow) | Gets the row index of the comment. |
| [getTextHorizontalAlignment()](#gettexthorizontalalignment) | Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer  |
| [getTextOrientationType()](#gettextorientationtype) | Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constan |
| [getTextVerticalAlignment()](#gettextverticalalignment) | Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer co |
| [getThreadedComments()](#getthreadedcomments) | Gets the list of threaded comments; |
| [getWidth()](#getwidth) | Represents the width of the comment, in unit of pixels. |
| [getWidthCM()](#getwidthcm) | Represents the width of the comment, in unit of centimeters. |
| [getWidthInch()](#getwidthinch) | Represents the width of the comment, in unit of inches. |
| [isThreadedComment()](#isthreadedcomment) | Indicates whether this comment is a threaded comment. |
| [isVisible()](#isvisible) | Represents if the comment is visible or not. |
| [setAuthor()](#setauthor) | Gets and sets Name of the original comment author |
| [setAutoSize()](#setautosize) | Indicates if size of comment is adjusted automatically according to its content. |
| [setHeight()](#setheight) | Represents the Height of the comment, in unit of pixels. |
| [setHeightCM()](#setheightcm) | Represents the height of the comment, in unit of centimeters. |
| [setHeightInch()](#setheightinch) | Represents the height of the comment, in unit of inches. |
| [setHtmlNote()](#sethtmlnote) | Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the n |
| [setNote()](#setnote) | Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel coul |
| [setTextHorizontalAlignment()](#settexthorizontalalignment) | Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer  |
| [setTextOrientationType()](#settextorientationtype) | Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constan |
| [setTextVerticalAlignment()](#settextverticalalignment) | Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer co |
| [setVisible()](#setvisible) | Represents if the comment is visible or not. |
| [setWidth()](#setwidth) | Represents the width of the comment, in unit of pixels. |
| [setWidthCM()](#setwidthcm) | Represents the width of the comment, in unit of centimeters. |
| [setWidthInch()](#setwidthinch) | Represents the width of the comment, in unit of inches. |

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the comment text.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** FontSetting — `FontSetting` Characters object.

### formatCharacters(startIndex, length, font, flag) {#formatcharacters}

Format some characters with the font setting.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The start index. |
| length | Number | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### getAuthor() {#getauthor}

Gets and sets Name of the original comment author

### getAutoSize() {#getautosize}

Indicates if size of comment is adjusted automatically according to its content.

### getColumn() {#getcolumn}

Gets the column index of the comment.

### getCommentShape() {#getcommentshape}

Get a Shape object that represents the shape attached to the specified comment.

### getFont() {#getfont}

Gets the font of comment.

### getHeight() {#getheight}

Represents the Height of the comment, in unit of pixels.

### getHeightCM() {#getheightcm}

Represents the height of the comment, in unit of centimeters.

### getHeightInch() {#getheightinch}

Represents the height of the comment, in unit of inches.

### getHtmlNote() {#gethtmlnote}

Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### getNote() {#getnote}

Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### getRichFormattings() {#getrichformattings}

Returns all Characters objects that represents a range of characters within the comment text.

**Returns:** Array ofFontSetting — `Array ofFontSetting` All Characters objects

### getRow() {#getrow}

Gets the row index of the comment.

### getTextHorizontalAlignment() {#gettexthorizontalalignment}

Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer constant.

### getTextOrientationType() {#gettextorientationtype}

Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constant.

### getTextVerticalAlignment() {#gettextverticalalignment}

Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer constant.

### getThreadedComments() {#getthreadedcomments}

Gets the list of threaded comments;

### getWidth() {#getwidth}

Represents the width of the comment, in unit of pixels.

### getWidthCM() {#getwidthcm}

Represents the width of the comment, in unit of centimeters.

### getWidthInch() {#getwidthinch}

Represents the width of the comment, in unit of inches.

### isThreadedComment() {#isthreadedcomment}

Indicates whether this comment is a threaded comment.

### isVisible() {#isvisible}

Represents if the comment is visible or not.

### setAuthor() {#setauthor}

Gets and sets Name of the original comment author

### setAutoSize() {#setautosize}

Indicates if size of comment is adjusted automatically according to its content.

### setHeight() {#setheight}

Represents the Height of the comment, in unit of pixels.

### setHeightCM() {#setheightcm}

Represents the height of the comment, in unit of centimeters.

### setHeightInch() {#setheightinch}

Represents the height of the comment, in unit of inches.

### setHtmlNote() {#sethtmlnote}

Gets and sets the html string which contains data and some formats in this comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### setNote() {#setnote}

Represents the content of comment. If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### setTextHorizontalAlignment() {#settexthorizontalalignment}

Gets and sets the text horizontal alignment type of the comment. The value of the property is TextAlignmentType integer constant.

### setTextOrientationType() {#settextorientationtype}

Gets and sets the text orientation type of the comment. The value of the property is TextOrientationType integer constant.

### setTextVerticalAlignment() {#settextverticalalignment}

Gets and sets the text vertical alignment type of the comment. The value of the property is TextAlignmentType integer constant.

### setVisible() {#setvisible}

Represents if the comment is visible or not.

### setWidth() {#setwidth}

Represents the width of the comment, in unit of pixels.

### setWidthCM() {#setwidthcm}

Represents the width of the comment, in unit of centimeters.

### setWidthInch() {#setwidthinch}

Represents the width of the comment, in unit of inches.
