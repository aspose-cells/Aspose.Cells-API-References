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
// Called: string au = tcs[0].Author.Name;
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

* class [ThreadedComment](../../threadedcomment/)
* class [ThreadedCommentCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


