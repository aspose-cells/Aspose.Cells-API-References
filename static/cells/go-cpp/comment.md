##Comment Class
'Comment class. Encapsulates the object that represents comment in Go.'
## Comment class
Encapsulates the object that represents a cell comment.
```go
type Comment struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[GetAuthor](./getauthor/) | Gets and sets Name of the original comment author |
|[SetAuthor](./setauthor/) | Gets and sets Name of the original comment author |
|[GetCommentShape](./getcommentshape/) | Get a Shape object that represents the shape attached to the specified comment. |
|[GetRow](./getrow/) | Gets the row index of the comment. |
|[GetColumn](./getcolumn/) | Gets the column index of the comment. |
|[IsThreadedComment](./isthreadedcomment/) | Indicates whether this comment is a threaded comment. |
|[GetThreadedComments](./getthreadedcomments/) | Gets the list of threaded comments; |
|[GetNote](./getnote/) | Represents the content of comment. |
|[SetNote](./setnote/) | Represents the content of comment. |
|[GetHtmlNote](./gethtmlnote/) | Gets and sets the html string which contains data and some formats in this comment. |
|[SetHtmlNote](./sethtmlnote/) | Gets and sets the html string which contains data and some formats in this comment. |
|[GetFont](./getfont/) | Gets the font of comment. |
|[FormatCharacters](./formatcharacters/) | Format some characters with the font setting. |
|[Characters](./characters/) | Returns a Characters object that represents a range of characters within the comment text. |
|[GetRichFormattings](./getrichformattings/) | Returns all Characters objectsthat represents a range of characters within the comment text. |
|[IsVisible](./isvisible/) | Represents if the comment is visible or not. |
|[SetIsVisible](./setisvisible/) | Represents if the comment is visible or not. |
|[GetTextOrientationType](./gettextorientationtype/) | Gets and sets the text orientation type of the comment. |
|[SetTextOrientationType](./settextorientationtype/) | Gets and sets the text orientation type of the comment. |
|[GetTextHorizontalAlignment](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the comment. |
|[SetTextHorizontalAlignment](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the comment. |
|[GetTextVerticalAlignment](./gettextverticalalignment/) | Gets and sets the text vertical alignment type of the comment. |
|[SetTextVerticalAlignment](./settextverticalalignment/) | Gets and sets the text vertical alignment type of the comment. |
|[GetAutoSize](./getautosize/) | Indicates if size of comment is adjusted automatically according to its content.Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
|[SetAutoSize](./setautosize/) | Indicates if size of comment is adjusted automatically according to its content.Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
|[GetHeightCM](./getheightcm/) | Represents the height of the comment, in unit of centimeters. |
|[SetHeightCM](./setheightcm/) | Represents the height of the comment, in unit of centimeters. |
|[GetWidthCM](./getwidthcm/) | Represents the width of the comment, in unit of centimeters. |
|[SetWidthCM](./setwidthcm/) | Represents the width of the comment, in unit of centimeters. |
|[GetWidth](./getwidth/) | Represents the width of the comment, in unit of pixels. |
|[SetWidth](./setwidth/) | Represents the width of the comment, in unit of pixels. |
|[GetHeight](./getheight/) | Represents the Height of the comment, in unit of pixels. |
|[SetHeight](./setheight/) | Represents the Height of the comment, in unit of pixels. |
|[GetWidthInch](./getwidthinch/) | Represents the width of the comment, in unit of inches. |
|[SetWidthInch](./setwidthinch/) | Represents the width of the comment, in unit of inches. |
|[GetHeightInch](./getheightinch/) | Represents the height of the comment, in unit of inches. |
|[SetHeightInch](./setheightinch/) | Represents the height of the comment, in unit of inches. |
