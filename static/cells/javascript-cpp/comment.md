##Comment
Encapsulates the object that represents a cell comment.
## Comment class
Encapsulates the object that represents a cell comment.
```javascript
class Comment;
```
### Example
```javascript
const { Workbook } = AsposeCells;
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
| [formatCharacters(number, number, Font, StyleFlag)](#formatCharacters-number-number-font-styleflag-)| Format some characters with the font setting. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the comment text. |
| [getRichFormattings()](#getRichFormattings--)| Returns all Characters objects that represents a range of characters within the comment text. |
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
