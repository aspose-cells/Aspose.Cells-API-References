---
title: Class Comment
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.Comment class. Encapsulates the object that represents a cell comment
type: docs
url: /net/aspose.cells/comment/
---
## Comment class

Encapsulates the object that represents a cell comment.

```csharp
public class Comment
```

## Properties

| Name | Description |
| --- | --- |
| [Author](../../aspose.cells/comment/author/) { get; set; } | Gets and sets Name of the original comment author |
| [AutoSize](../../aspose.cells/comment/autosize/) { get; set; } | Indicates if size of comment is adjusted automatically according to its content. Note: In some special cases (such as Mac environment), this setting may not take effect. If this setting does not take effect, please replace it with FitToTextSize(). |
| [Column](../../aspose.cells/comment/column/) { get; } | Gets the column index of the comment. |
| [CommentShape](../../aspose.cells/comment/commentshape/) { get; } | Get a Shape object that represents the shape attached to the specified comment. |
| [Font](../../aspose.cells/comment/font/) { get; } | Gets the font of comment. |
| [Height](../../aspose.cells/comment/height/) { get; set; } | Represents the Height of the comment, in unit of pixels. |
| [HeightCM](../../aspose.cells/comment/heightcm/) { get; set; } | Represents the height of the comment, in unit of centimeters. |
| [HeightInch](../../aspose.cells/comment/heightinch/) { get; set; } | Represents the height of the comment, in unit of inches. |
| [HtmlNote](../../aspose.cells/comment/htmlnote/) { get; set; } | Gets and sets the html string which contains data and some formats in this comment. |
| [IsThreadedComment](../../aspose.cells/comment/isthreadedcomment/) { get; } | Indicates whether this comment is a threaded comment. |
| [IsVisible](../../aspose.cells/comment/isvisible/) { get; set; } | Represents if the comment is visible or not. |
| [Note](../../aspose.cells/comment/note/) { get; set; } | Represents the content of comment. |
| [Row](../../aspose.cells/comment/row/) { get; } | Gets the row index of the comment. |
| [TextHorizontalAlignment](../../aspose.cells/comment/texthorizontalalignment/) { get; set; } | Gets and sets the text horizontal alignment type of the comment. |
| [TextOrientationType](../../aspose.cells/comment/textorientationtype/) { get; set; } | Gets and sets the text orientation type of the comment. |
| [TextVerticalAlignment](../../aspose.cells/comment/textverticalalignment/) { get; set; } | Gets and sets the text vertical alignment type of the comment. |
| [ThreadedComments](../../aspose.cells/comment/threadedcomments/) { get; } | Gets the list of threaded comments; |
| [Width](../../aspose.cells/comment/width/) { get; set; } | Represents the width of the comment, in unit of pixels. |
| [WidthCM](../../aspose.cells/comment/widthcm/) { get; set; } | Represents the width of the comment, in unit of centimeters. |
| [WidthInch](../../aspose.cells/comment/widthinch/) { get; set; } | Represents the width of the comment, in unit of inches. |

## Methods

| Name | Description |
| --- | --- |
| [Characters](../../aspose.cells/comment/characters/)(int, int) | Returns a Characters object that represents a range of characters within the comment text. |
| [FormatCharacters](../../aspose.cells/comment/formatcharacters/)(int, int, Font, StyleFlag) | Format some characters with the font setting. |
| [GetCharacters](../../aspose.cells/comment/getcharacters/)() | (**Obsolete.**) Returns all Characters objects that represents a range of characters within the comment text. |
| [GetRichFormattings](../../aspose.cells/comment/getrichformattings/)() | Returns all Characters objects that represents a range of characters within the comment text. |

### Examples

```csharp
[C#]

Workbook workbook = new Workbook();
CommentCollection comments = workbook.Worksheets[0].Comments;

//Add comment to cell A1
int commentIndex1 = comments.Add(0, 0);
Comment comment1 = comments[commentIndex1];
comment1.Note = "First note.";
comment1.Font.Name = "Times New Roman";

//Add comment to cell B2
comments.Add("B2");
Comment comment2 = comments["B2"];
comment2.Note = "Second note.";

//do your business

//Save the excel file.
workbook.Save("exmaple.xlsx");

[Visual Basic]

Dim workbook as Workbook = new Workbook()
Dim comments as CommentCollection = workbook.Worksheets(0).Comments
 
'Add comment to cell A1
Dim commentIndex1 as Integer = comments.Add(0, 0)
Dim comment1 as Comment = comments(commentIndex1)
comment1.Note = "First note."
comment1.Font.Name = "Times New Roman"

'Add comment to cell B2
comments.Add("B2")
Dim comment2 As Comment = comments("B2")
comment2.Note = "Second note."
 
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


