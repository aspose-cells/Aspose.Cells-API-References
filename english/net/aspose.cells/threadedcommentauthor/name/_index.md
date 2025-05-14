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
public void ThreadedCommentAuthor_Property_Name()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
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
    workbook.Save(Constants.destPath + "example.xlsx");

}
```

### See Also

* class [ThreadedCommentAuthor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


