---
title: Comment
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Encapsulates the object that represents a cell comment.
type: docs
url: /nodejs-cpp/comment/
---

## Comment class

Encapsulates the object that represents a cell comment.

```javascript
class Comment;
```


## Methods

| Method | Description |
| --- | --- |
| [getAuthor()](#getAuthor--)| Gets and sets Name of the original comment author |
| [setAuthor(string)](#setAuthor-string-)| Gets and sets Name of the original comment author |
| [getCommentShape()](#getCommentShape--)| Get a Shape object that represents the shape attached to the specified comment. |
| [getRow()](#getRow--)| Gets the row index of the comment. |
| [getColumn()](#getColumn--)| Gets the column index of the comment. |
| [isThreadedComment()](#isThreadedComment--)| Indicates whether this comment is a threaded comment. |
| [getThreadedComments()](#getThreadedComments--)| Gets the list of threaded comments; |
| [getNote()](#getNote--)| Represents the content of comment. |
| [setNote(string)](#setNote-string-)| Represents the content of comment. |
| [getHtmlNote()](#getHtmlNote--)| Gets and sets the html string which contains data and some formats in this comment. |
| [setHtmlNote(string)](#setHtmlNote-string-)| Gets and sets the html string which contains data and some formats in this comment. |
| [getFont()](#getFont--)| Gets the font of comment. |
| [isVisible()](#isVisible--)| Represents if the comment is visible or not. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| Represents if the comment is visible or not. |
| [getTextOrientationType()](#getTextOrientationType--)| Gets and sets the text orientation type of the comment. |
| [setTextOrientationType(TextOrientationType)](#setTextOrientationType-textorientationtype-)| Gets and sets the text orientation type of the comment. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| Gets and sets the text horizontal alignment type of the comment. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| Gets and sets the text horizontal alignment type of the comment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| Gets and sets the text vertical alignment type of the comment. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| Gets and sets the text vertical alignment type of the comment. |
| [getAutoSize()](#getAutoSize--)| Indicates if size of comment is adjusted automatically according to its content. |
| [setAutoSize(boolean)](#setAutoSize-boolean-)| Indicates if size of comment is adjusted automatically according to its content. |
| [getHeightCM()](#getHeightCM--)| Represents the height of the comment, in unit of centimeters. |
| [setHeightCM(number)](#setHeightCM-number-)| Represents the height of the comment, in unit of centimeters. |
| [getWidthCM()](#getWidthCM--)| Represents the width of the comment, in unit of centimeters. |
| [setWidthCM(number)](#setWidthCM-number-)| Represents the width of the comment, in unit of centimeters. |
| [getWidth()](#getWidth--)| Represents the width of the comment, in unit of pixels. |
| [setWidth(number)](#setWidth-number-)| Represents the width of the comment, in unit of pixels. |
| [getHeight()](#getHeight--)| Represents the Height of the comment, in unit of pixels. |
| [setHeight(number)](#setHeight-number-)| Represents the Height of the comment, in unit of pixels. |
| [getWidthInch()](#getWidthInch--)| Represents the width of the comment, in unit of inches. |
| [setWidthInch(number)](#setWidthInch-number-)| Represents the width of the comment, in unit of inches. |
| [getHeightInch()](#getHeightInch--)| Represents the height of the comment, in unit of inches. |
| [setHeightInch(number)](#setHeightInch-number-)| Represents the height of the comment, in unit of inches. |
| [formatCharacters(number, number, Font, StyleFlag)](#formatCharacters-number-number-font-styleflag-)| Format some characters with the font setting. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the comment text. |
| [getRichFormattings()](#getRichFormattings--)| Returns all Characters objects that represents a range of characters within the comment text. |


### getAuthor() {#getAuthor--}

Gets and sets Name of the original comment author

```javascript
getAuthor() : string;
```


### setAuthor(string) {#setAuthor-string-}

Gets and sets Name of the original comment author

```javascript
setAuthor(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getCommentShape() {#getCommentShape--}

Get a Shape object that represents the shape attached to the specified comment.

```javascript
getCommentShape() : CommentShape;
```


**Returns**

[CommentShape](./commentshape/)

### getRow() {#getRow--}

Gets the row index of the comment.

```javascript
getRow() : number;
```


### getColumn() {#getColumn--}

Gets the column index of the comment.

```javascript
getColumn() : number;
```


### isThreadedComment() {#isThreadedComment--}

Indicates whether this comment is a threaded comment.

```javascript
isThreadedComment() : boolean;
```


### getThreadedComments() {#getThreadedComments--}

Gets the list of threaded comments;

```javascript
getThreadedComments() : ThreadedCommentCollection;
```


**Returns**

[ThreadedCommentCollection](./threadedcommentcollection/)

### getNote() {#getNote--}

Represents the content of comment.

```javascript
getNote() : string;
```


**Remarks**

If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### setNote(string) {#setNote-string-}

Represents the content of comment.

```javascript
setNote(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### getHtmlNote() {#getHtmlNote--}

Gets and sets the html string which contains data and some formats in this comment.

```javascript
getHtmlNote() : string;
```


**Remarks**

If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### setHtmlNote(string) {#setHtmlNote-string-}

Gets and sets the html string which contains data and some formats in this comment.

```javascript
setHtmlNote(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

**Remarks**

If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.

### getFont() {#getFont--}

Gets the font of comment.

```javascript
getFont() : Font;
```


**Returns**

[Font](./font/)

### isVisible() {#isVisible--}

Represents if the comment is visible or not.

```javascript
isVisible() : boolean;
```


### setIsVisible(boolean) {#setIsVisible-boolean-}

Represents if the comment is visible or not.

```javascript
setIsVisible(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextOrientationType() {#getTextOrientationType--}

Gets and sets the text orientation type of the comment.

```javascript
getTextOrientationType() : TextOrientationType;
```


**Returns**

[TextOrientationType](./textorientationtype/)

### setTextOrientationType(TextOrientationType) {#setTextOrientationType-textorientationtype-}

Gets and sets the text orientation type of the comment.

```javascript
setTextOrientationType(value: TextOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOrientationType](./textorientationtype/) | The value to set. |

### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}

Gets and sets the text horizontal alignment type of the comment.

```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](./textalignmenttype/)

### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}

Gets and sets the text horizontal alignment type of the comment.

```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](./textalignmenttype/) | The value to set. |

### getTextVerticalAlignment() {#getTextVerticalAlignment--}

Gets and sets the text vertical alignment type of the comment.

```javascript
getTextVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](./textalignmenttype/)

### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}

Gets and sets the text vertical alignment type of the comment.

```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](./textalignmenttype/) | The value to set. |

### getAutoSize() {#getAutoSize--}

Indicates if size of comment is adjusted automatically according to its content.

```javascript
getAutoSize() : boolean;
```


### setAutoSize(boolean) {#setAutoSize-boolean-}

Indicates if size of comment is adjusted automatically according to its content.

```javascript
setAutoSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getHeightCM() {#getHeightCM--}

Represents the height of the comment, in unit of centimeters.

```javascript
getHeightCM() : number;
```


### setHeightCM(number) {#setHeightCM-number-}

Represents the height of the comment, in unit of centimeters.

```javascript
setHeightCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthCM() {#getWidthCM--}

Represents the width of the comment, in unit of centimeters.

```javascript
getWidthCM() : number;
```


### setWidthCM(number) {#setWidthCM-number-}

Represents the width of the comment, in unit of centimeters.

```javascript
setWidthCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidth() {#getWidth--}

Represents the width of the comment, in unit of pixels.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

Represents the width of the comment, in unit of pixels.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeight() {#getHeight--}

Represents the Height of the comment, in unit of pixels.

```javascript
getHeight() : number;
```


### setHeight(number) {#setHeight-number-}

Represents the Height of the comment, in unit of pixels.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthInch() {#getWidthInch--}

Represents the width of the comment, in unit of inches.

```javascript
getWidthInch() : number;
```


### setWidthInch(number) {#setWidthInch-number-}

Represents the width of the comment, in unit of inches.

```javascript
setWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightInch() {#getHeightInch--}

Represents the height of the comment, in unit of inches.

```javascript
getHeightInch() : number;
```


### setHeightInch(number) {#setHeightInch-number-}

Represents the height of the comment, in unit of inches.

```javascript
setHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### formatCharacters(number, number, Font, StyleFlag) {#formatCharacters-number-number-font-styleflag-}

Format some characters with the font setting.

```javascript
formatCharacters(startIndex: number, length: number, font: Font, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The start index. |
| length | number | The length. |
| font | [Font](./font/) | The font setting. |
| flag | [StyleFlag](./styleflag/) | The flag of the font setting. |

### characters(number, number) {#characters-number-number-}

Returns a Characters object that represents a range of characters within the comment text.

```javascript
characters(startIndex: number, length: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |

**Returns**

Characters object.

### getRichFormattings() {#getRichFormattings--}

Returns all Characters objects that represents a range of characters within the comment text.

```javascript
getRichFormattings() : FontSetting[];
```


**Returns**

All Characters objects


