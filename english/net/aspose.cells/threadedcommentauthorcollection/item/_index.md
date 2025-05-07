---
title: ThreadedCommentAuthorCollection.Item
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthorCollection property. Gets the person who create threaded comments
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/item/
---
## ThreadedCommentAuthorCollection indexer (1 of 2)

Gets the person who create threaded comments.

```csharp
public ThreadedCommentAuthor this[int index] { get; }
```

| Parameter | Description |
| --- | --- |
| index | The index |

### Examples

```csharp
// Called: tcs[1].Author = authors[index];
[Test]
        public void Property_Int32_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNETCORE233.xlsx");
            Worksheet worksheet = workbook.Worksheets[0];
            CommentCollection comments = worksheet.Comments;
            Comment comment = comments[0];
            ThreadedCommentCollection tcs = comment.ThreadedComments;
            Assert.AreEqual(2, tcs.Count);
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            string au = tcs[0].Author.Name;
           int index = authors.Add("Aspose", "S::johnson.shi@asposenj.onmicrosoft.com::bd07c1a8-5f37-4ecf-bd20-1f831c9015ce", "AD");

            tcs[1].Author = authors[index];
            Assert.AreEqual(au, tcs[0].Author.Name);
            Assert.AreEqual("Aspose", tcs[1].Author.Name);
            workbook.Save(Constants.destPath + "CELLSNETCORE233.xlsx");

        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## ThreadedCommentAuthorCollection indexer (2 of 2)

Gets the person who create threaded comments.

```csharp
public ThreadedCommentAuthor this[string name] { get; }
```

| Parameter | Description |
| --- | --- |
| name | The name of the author. |

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


