---
title: ThreadedCommentAuthor.Name
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthor property. Gets and sets the name
type: docs
url: /net/aspose.cells/threadedcommentauthor/name/
---
## ThreadedCommentAuthor.Name property

Gets and sets the name.

```csharp
public string Name { get; set; }
```

### Examples

```csharp
// Called: string au = tcs[0].Author.Name;
[Test]
        public void Property_Name()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNETCORE233.xlsx&quot;);
            Worksheet worksheet = workbook.Worksheets[0];
            CommentCollection comments = worksheet.Comments;
            Comment comment = comments[0];
            ThreadedCommentCollection tcs = comment.ThreadedComments;
            Assert.AreEqual(2, tcs.Count);
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            string au = tcs[0].Author.Name;
           int index = authors.Add(&quot;Aspose&quot;, &quot;S::johnson.shi@asposenj.onmicrosoft.com::bd07c1a8-5f37-4ecf-bd20-1f831c9015ce&quot;, &quot;AD&quot;);

            tcs[1].Author = authors[index];
            Assert.AreEqual(au, tcs[0].Author.Name);
            Assert.AreEqual(&quot;Aspose&quot;, tcs[1].Author.Name);
            workbook.Save(Constants.destPath + &quot;CELLSNETCORE233.xlsx&quot;);

        }
```

### See Also

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


