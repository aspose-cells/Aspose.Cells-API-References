---
title: Class ThreadedCommentAuthor
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedCommentAuthor class. Represents the person who creates the threaded comments
type: docs
url: /net/aspose.cells/threadedcommentauthor/
---
## ThreadedCommentAuthor class

Represents the person who creates the threaded comments;

```csharp
public class ThreadedCommentAuthor
```

## Properties

| Name | Description |
| --- | --- |
| [Name](../../aspose.cells/threadedcommentauthor/name/) { get; set; } | Gets and sets the name. |
| [ProviderId](../../aspose.cells/threadedcommentauthor/providerid/) { get; set; } | Gets the id of the provider. |
| [UserId](../../aspose.cells/threadedcommentauthor/userid/) { get; set; } | Gets and sets the id of the user. |

### Examples

```csharp
// Called: ThreadedCommentAuthor author = tcs[0].Author;
public void Cells_Type_ThreadedCommentAuthor()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = workbook.Worksheets[0];
    CommentCollection comments = worksheet.Comments;
    Comment comment = comments[0];
    ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
    ThreadedCommentCollection tcs = comment.ThreadedComments;
    string au = tcs[0].Author.Name;
    tcs[0].Author.Name = "Cells";
    Assert.AreEqual(au, tcs[0].Author.Name);
    ThreadedCommentAuthor author = tcs[0].Author;
    author.Name = "Cells";
    tcs[0].Author = author;
    Assert.AreEqual("Cells", tcs[0].Author.Name);
}
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


