##Aspose::Cells::Comment class
'Aspose::Cells::Comment class. Encapsulates the object that represents a cell comment in C++.'
## Comment class
Encapsulates the object that represents a cell comment.
```cpp
class Comment
```
## Methods
| Method | Description |
| --- | --- |
| [Characters(int32_t startIndex, int32_t length)](./characters/) | Returns a Characters object that represents a range of characters within the comment text. |
| [Comment(Comment_Impl* impl)](./comment/) | Constructs from an implementation object. |
| [Comment(const Comment\& src)](./comment/) | Copy constructor. |
| [FormatCharacters(int32_t startIndex, int32_t length, const Aspose::Cells::Font\& font, const StyleFlag\& flag)](./formatcharacters/) | Format some characters with the font setting. |
| [GetAuthor()](./getauthor/) | Gets and sets [Name](../name/) of the original comment author. |
| [GetAutoSize()](./getautosize/) | Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [GetColumn()](./getcolumn/) | Gets the column index of the comment. |
| [GetCommentShape()](./getcommentshape/) | Get a Shape object that represents the shape attached to the specified comment. |
| [GetFont()](./getfont/) | Gets the font of comment. |
| [GetHeight()](./getheight/) | Represents the Height of the comment, in unit of pixels. |
| [GetHeightCM()](./getheightcm/) | Represents the height of the comment, in unit of centimeters. |
| [GetHeightInch()](./getheightinch/) | Represents the height of the comment, in unit of inches. |
| [GetHtmlNote()](./gethtmlnote/) | Gets and sets the html string which contains data and some formats in this comment. |
| [GetNote()](./getnote/) | Represents the content of comment. |
| [GetRichFormattings()](./getrichformattings/) | Returns all Characters objects that represents a range of characters within the comment text. |
| [GetRow()](./getrow/) | Gets the row index of the comment. |
| [GetTextHorizontalAlignment()](./gettexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the comment. |
| [GetTextOrientationType()](./gettextorientationtype/) | Gets and sets the text orientation type of the comment. |
| [GetTextVerticalAlignment()](./gettextverticalalignment/) | Gets and sets the text vertical alignment type of the comment. |
| [GetThreadedComments()](./getthreadedcomments/) | Gets the list of threaded comments;. |
| [GetWidth()](./getwidth/) | Represents the width of the comment, in unit of pixels. |
| [GetWidthCM()](./getwidthcm/) | Represents the width of the comment, in unit of centimeters. |
| [GetWidthInch()](./getwidthinch/) | Represents the width of the comment, in unit of inches. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsThreadedComment()](./isthreadedcomment/) | Indicates whether this comment is a threaded comment. |
| [IsVisible()](./isvisible/) | Represents if the comment is visible or not. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Comment\& src)](./operator_asm/) | operator= |
| [SetAuthor(const U16String\& value)](./setauthor/) | Gets and sets [Name](../name/) of the original comment author. |
| [SetAuthor(const char16_t* value)](./setauthor/) | Gets and sets [Name](../name/) of the original comment author. |
| [SetAutoSize(bool value)](./setautosize/) | Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [SetHeight(int32_t value)](./setheight/) | Represents the Height of the comment, in unit of pixels. |
| [SetHeightCM(double value)](./setheightcm/) | Represents the height of the comment, in unit of centimeters. |
| [SetHeightInch(double value)](./setheightinch/) | Represents the height of the comment, in unit of inches. |
| [SetHtmlNote(const U16String\& value)](./sethtmlnote/) | Gets and sets the html string which contains data and some formats in this comment. |
| [SetHtmlNote(const char16_t* value)](./sethtmlnote/) | Gets and sets the html string which contains data and some formats in this comment. |
| [SetIsVisible(bool value)](./setisvisible/) | Represents if the comment is visible or not. |
| [SetNote(const U16String\& value)](./setnote/) | Represents the content of comment. |
| [SetNote(const char16_t* value)](./setnote/) | Represents the content of comment. |
| [SetTextHorizontalAlignment(TextAlignmentType value)](./settexthorizontalalignment/) | Gets and sets the text horizontal alignment type of the comment. |
| [SetTextOrientationType(TextOrientationType value)](./settextorientationtype/) | Gets and sets the text orientation type of the comment. |
| [SetTextVerticalAlignment(TextAlignmentType value)](./settextverticalalignment/) | Gets and sets the text vertical alignment type of the comment. |
| [SetWidth(int32_t value)](./setwidth/) | Represents the width of the comment, in unit of pixels. |
| [SetWidthCM(double value)](./setwidthcm/) | Represents the width of the comment, in unit of centimeters. |
| [SetWidthInch(double value)](./setwidthinch/) | Represents the width of the comment, in unit of inches. |
| [~Comment()](./~comment/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
Workbook workbook;
CommentCollection comments = workbook.GetWorksheets().Get(0).GetComments();
//Add comment to cell A1
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments.Get(commentIndex1);
comment1.SetNote(u"First note.");
comment1.GetFont().SetName(u"Times New Roman");
//Add comment to cell B2
comments.Add(u"B2");
Comment comment2 = comments.Get("B2");
comment2.SetNote(u"Second note.");
//Save the excel file.
workbook.Save(u"exmaple.xlsx");
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
