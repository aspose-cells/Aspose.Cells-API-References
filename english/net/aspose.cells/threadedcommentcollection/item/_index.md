---
title: ThreadedCommentCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentCollection property. Gets the threaded comment by the specific index
type: docs
url: /net/aspose.cells/threadedcommentcollection/item/
---
## ThreadedCommentCollection indexer

Gets the threaded comment by the specific index.

```csharp
public ThreadedComment this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Examples

```csharp
// Called: ThreadedCommentAuthor author = tcs[0].Author;
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNETCORE245.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            CommentCollection comments = worksheet.Comments;
            Comment comment = comments[0];
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            ThreadedCommentCollection tcs = comment.ThreadedComments;
            string au = tcs[0].Author.Name;
            tcs[0].Author.Name = &quot;Cells&quot;;
            Assert.AreEqual(au, tcs[0].Author.Name);
            ThreadedCommentAuthor author = tcs[0].Author;
            author.Name = &quot;Cells&quot;;
            tcs[0].Author = author;
            Assert.AreEqual(&quot;Cells&quot;, tcs[0].Author.Name);
        }
```

### See Also

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


