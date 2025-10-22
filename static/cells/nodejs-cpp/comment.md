##Comment
Encapsulates the object that represents a cell comment.
## Comment class
Encapsulates the object that represents a cell comment.
```javascript
class Comment;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var workbook = new Workbook();
var comments = workbook.worksheets.get(0).comments;
//Add comment to cell A1
var commentIndex = comments.add(0, 0);
var comment = comments.get(commentIndex);
comment.note = "First note.";
comment.font.setName("Times New Roman");
//Add comment to cell B2
comments.add("B2");
comment = comments.get("B2");
comment.note = "Second note.";
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [author](#author--)| string | Gets and sets Name of the original comment author |
| [commentShape](#commentShape--)| CommentShape | Readonly. Get a Shape object that represents the shape attached to the specified comment. |
| [row](#row--)| number | Readonly. Gets the row index of the comment. |
| [column](#column--)| number | Readonly. Gets the column index of the comment. |
| [isThreadedComment](#isThreadedComment--)| boolean | Readonly. Indicates whether this comment is a threaded comment. |
| [threadedComments](#threadedComments--)| ThreadedCommentCollection | Readonly. Gets the list of threaded comments; |
| [note](#note--)| string | Represents the content of comment. |
| [htmlNote](#htmlNote--)| string | Gets and sets the html string which contains data and some formats in this comment. |
| [font](#font--)| Font | Readonly. Gets the font of comment. |
| [isVisible](#isVisible--)| boolean | Represents if the comment is visible or not. |
| [textOrientationType](#textOrientationType--)| TextOrientationType | Gets and sets the text orientation type of the comment. |
| [textHorizontalAlignment](#textHorizontalAlignment--)| TextAlignmentType | Gets and sets the text horizontal alignment type of the comment. |
| [textVerticalAlignment](#textVerticalAlignment--)| TextAlignmentType | Gets and sets the text vertical alignment type of the comment. |
| [autoSize](#autoSize--)| boolean | Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [heightCM](#heightCM--)| number | Represents the height of the comment, in unit of centimeters. |
| [widthCM](#widthCM--)| number | Represents the width of the comment, in unit of centimeters. |
| [width](#width--)| number | Represents the width of the comment, in unit of pixels. |
| [height](#height--)| number | Represents the Height of the comment, in unit of pixels. |
| [widthInch](#widthInch--)| number | Represents the width of the comment, in unit of inches. |
| [heightInch](#heightInch--)| number | Represents the height of the comment, in unit of inches. |
## Methods
| Method | Description |
| --- | --- |
| [getAuthor()](#getAuthor--)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets Name of the original comment author |
| [setAuthor(string)](#setAuthor-string-)| <b>@deprecated.</b> Please use the 'author' property instead. Gets and sets Name of the original comment author |
| [getCommentShape()](#getCommentShape--)| <b>@deprecated.</b> Please use the 'commentShape' property instead. Get a Shape object that represents the shape attached to the specified comment. |
| [getRow()](#getRow--)| <b>@deprecated.</b> Please use the 'row' property instead. Gets the row index of the comment. |
| [getColumn()](#getColumn--)| <b>@deprecated.</b> Please use the 'column' property instead. Gets the column index of the comment. |
| [isThreadedComment()](#isThreadedComment--)| <b>@deprecated.</b> Please use the 'isThreadedComment' property instead. Indicates whether this comment is a threaded comment. |
| [getThreadedComments()](#getThreadedComments--)| <b>@deprecated.</b> Please use the 'threadedComments' property instead. Gets the list of threaded comments; |
| [getNote()](#getNote--)| <b>@deprecated.</b> Please use the 'note' property instead. Represents the content of comment. |
| [setNote(string)](#setNote-string-)| <b>@deprecated.</b> Please use the 'note' property instead. Represents the content of comment. |
| [getHtmlNote()](#getHtmlNote--)| <b>@deprecated.</b> Please use the 'htmlNote' property instead. Gets and sets the html string which contains data and some formats in this comment. |
| [setHtmlNote(string)](#setHtmlNote-string-)| <b>@deprecated.</b> Please use the 'htmlNote' property instead. Gets and sets the html string which contains data and some formats in this comment. |
| [getFont()](#getFont--)| <b>@deprecated.</b> Please use the 'font' property instead. Gets the font of comment. |
| [isVisible()](#isVisible--)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents if the comment is visible or not. |
| [setIsVisible(boolean)](#setIsVisible-boolean-)| <b>@deprecated.</b> Please use the 'isVisible' property instead. Represents if the comment is visible or not. |
| [getTextOrientationType()](#getTextOrientationType--)| <b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the comment. |
| [setTextOrientationType(TextOrientationType)](#setTextOrientationType-textorientationtype-)| <b>@deprecated.</b> Please use the 'textOrientationType' property instead. Gets and sets the text orientation type of the comment. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the comment. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textHorizontalAlignment' property instead. Gets and sets the text horizontal alignment type of the comment. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the comment. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| <b>@deprecated.</b> Please use the 'textVerticalAlignment' property instead. Gets and sets the text vertical alignment type of the comment. |
| [getAutoSize()](#getAutoSize--)| <b>@deprecated.</b> Please use the 'autoSize' property instead. Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [setAutoSize(boolean)](#setAutoSize-boolean-)| <b>@deprecated.</b> Please use the 'autoSize' property instead. Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [getHeightCM()](#getHeightCM--)| <b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the comment, in unit of centimeters. |
| [setHeightCM(number)](#setHeightCM-number-)| <b>@deprecated.</b> Please use the 'heightCM' property instead. Represents the height of the comment, in unit of centimeters. |
| [getWidthCM()](#getWidthCM--)| <b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the comment, in unit of centimeters. |
| [setWidthCM(number)](#setWidthCM-number-)| <b>@deprecated.</b> Please use the 'widthCM' property instead. Represents the width of the comment, in unit of centimeters. |
| [getWidth()](#getWidth--)| <b>@deprecated.</b> Please use the 'width' property instead. Represents the width of the comment, in unit of pixels. |
| [setWidth(number)](#setWidth-number-)| <b>@deprecated.</b> Please use the 'width' property instead. Represents the width of the comment, in unit of pixels. |
| [getHeight()](#getHeight--)| <b>@deprecated.</b> Please use the 'height' property instead. Represents the Height of the comment, in unit of pixels. |
| [setHeight(number)](#setHeight-number-)| <b>@deprecated.</b> Please use the 'height' property instead. Represents the Height of the comment, in unit of pixels. |
| [getWidthInch()](#getWidthInch--)| <b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the comment, in unit of inches. |
| [setWidthInch(number)](#setWidthInch-number-)| <b>@deprecated.</b> Please use the 'widthInch' property instead. Represents the width of the comment, in unit of inches. |
| [getHeightInch()](#getHeightInch--)| <b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the comment, in unit of inches. |
| [setHeightInch(number)](#setHeightInch-number-)| <b>@deprecated.</b> Please use the 'heightInch' property instead. Represents the height of the comment, in unit of inches. |
| [formatCharacters(number, number, Font, StyleFlag)](#formatCharacters-number-number-font-styleflag-)| Format some characters with the font setting. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the comment text. |
| [getRichFormattings()](#getRichFormattings--)| Returns all Characters objects that represents a range of characters within the comment text. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### author {#author--}
Gets and sets Name of the original comment author
```javascript
author : string;
```
### commentShape {#commentShape--}
Readonly. Get a Shape object that represents the shape attached to the specified comment.
```javascript
commentShape : CommentShape;
```
### row {#row--}
Readonly. Gets the row index of the comment.
```javascript
row : number;
```
### column {#column--}
Readonly. Gets the column index of the comment.
```javascript
column : number;
```
### isThreadedComment {#isThreadedComment--}
Readonly. Indicates whether this comment is a threaded comment.
```javascript
isThreadedComment : boolean;
```
### threadedComments {#threadedComments--}
Readonly. Gets the list of threaded comments;
```javascript
threadedComments : ThreadedCommentCollection;
```
### note {#note--}
Represents the content of comment.
```javascript
note : string;
```
**Remarks**
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### htmlNote {#htmlNote--}
Gets and sets the html string which contains data and some formats in this comment.
```javascript
htmlNote : string;
```
**Remarks**
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### font {#font--}
Readonly. Gets the font of comment.
```javascript
font : Font;
```
### isVisible {#isVisible--}
Represents if the comment is visible or not.
```javascript
isVisible : boolean;
```
### textOrientationType {#textOrientationType--}
Gets and sets the text orientation type of the comment.
```javascript
textOrientationType : TextOrientationType;
```
### textHorizontalAlignment {#textHorizontalAlignment--}
Gets and sets the text horizontal alignment type of the comment.
```javascript
textHorizontalAlignment : TextAlignmentType;
```
### textVerticalAlignment {#textVerticalAlignment--}
Gets and sets the text vertical alignment type of the comment.
```javascript
textVerticalAlignment : TextAlignmentType;
```
### autoSize {#autoSize--}
Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize().
```javascript
autoSize : boolean;
```
### heightCM {#heightCM--}
Represents the height of the comment, in unit of centimeters.
```javascript
heightCM : number;
```
### widthCM {#widthCM--}
Represents the width of the comment, in unit of centimeters.
```javascript
widthCM : number;
```
### width {#width--}
Represents the width of the comment, in unit of pixels.
```javascript
width : number;
```
### height {#height--}
Represents the Height of the comment, in unit of pixels.
```javascript
height : number;
```
### widthInch {#widthInch--}
Represents the width of the comment, in unit of inches.
```javascript
widthInch : number;
```
### heightInch {#heightInch--}
Represents the height of the comment, in unit of inches.
```javascript
heightInch : number;
```
### getAuthor() {#getAuthor--}
```javascript
getAuthor() : string;
```
### setAuthor(string) {#setAuthor-string-}
```javascript
setAuthor(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCommentShape() {#getCommentShape--}
```javascript
getCommentShape() : CommentShape;
```
**Returns**
[CommentShape](../commentshape/)
### getRow() {#getRow--}
```javascript
getRow() : number;
```
### getColumn() {#getColumn--}
```javascript
getColumn() : number;
```
### isThreadedComment() {#isThreadedComment--}
```javascript
isThreadedComment() : boolean;
```
### getThreadedComments() {#getThreadedComments--}
```javascript
getThreadedComments() : ThreadedCommentCollection;
```
**Returns**
[ThreadedCommentCollection](../threadedcommentcollection/)
### getNote() {#getNote--}
```javascript
getNote() : string;
```
**Remarks**
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### setNote(string) {#setNote-string-}
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
```javascript
getHtmlNote() : string;
```
**Remarks**
If this is a threaded comment, the note could not be changed, otherwise MS Excel could not process it as a threaded comment.
### setHtmlNote(string) {#setHtmlNote-string-}
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
```javascript
getFont() : Font;
```
**Returns**
[Font](../font/)
### isVisible() {#isVisible--}
```javascript
isVisible() : boolean;
```
### setIsVisible(boolean) {#setIsVisible-boolean-}
```javascript
setIsVisible(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getTextOrientationType() {#getTextOrientationType--}
```javascript
getTextOrientationType() : TextOrientationType;
```
**Returns**
[TextOrientationType](../textorientationtype/)
### setTextOrientationType(TextOrientationType) {#setTextOrientationType-textorientationtype-}
```javascript
setTextOrientationType(value: TextOrientationType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOrientationType](../textorientationtype/) | The value to set. |
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}
```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```javascript
getTextVerticalAlignment() : TextAlignmentType;
```
**Returns**
[TextAlignmentType](../textalignmenttype/)
### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}
```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](../textalignmenttype/) | The value to set. |
### getAutoSize() {#getAutoSize--}
```javascript
getAutoSize() : boolean;
```
### setAutoSize(boolean) {#setAutoSize-boolean-}
```javascript
setAutoSize(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getHeightCM() {#getHeightCM--}
```javascript
getHeightCM() : number;
```
### setHeightCM(number) {#setHeightCM-number-}
```javascript
setHeightCM(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWidthCM() {#getWidthCM--}
```javascript
getWidthCM() : number;
```
### setWidthCM(number) {#setWidthCM-number-}
```javascript
setWidthCM(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWidth() {#getWidth--}
```javascript
getWidth() : number;
```
### setWidth(number) {#setWidth-number-}
```javascript
setWidth(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeight() {#getHeight--}
```javascript
getHeight() : number;
```
### setHeight(number) {#setHeight-number-}
```javascript
setHeight(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getWidthInch() {#getWidthInch--}
```javascript
getWidthInch() : number;
```
### setWidthInch(number) {#setWidthInch-number-}
```javascript
setWidthInch(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getHeightInch() {#getHeightInch--}
```javascript
getHeightInch() : number;
```
### setHeightInch(number) {#setHeightInch-number-}
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
| font | [Font](../font/) | The font setting. |
| flag | [StyleFlag](../styleflag/) | The flag of the font setting. |
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
