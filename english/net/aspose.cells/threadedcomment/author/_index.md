---
title: ThreadedComment.Author
second_title: Aspose.Cells for .NET API Reference
description: ThreadedComment property. Gets the author of the comment
type: docs
url: /net/aspose.cells/threadedcomment/author/
---
## ThreadedComment.Author property

Gets the author of the comment.

```csharp
public ThreadedCommentAuthor Author { get; set; }
```

### Examples

```csharp
// Called: tcs[0].Author = author;
[Test]
        public void Property_Author()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNETCORE245.xlsx");
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

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


