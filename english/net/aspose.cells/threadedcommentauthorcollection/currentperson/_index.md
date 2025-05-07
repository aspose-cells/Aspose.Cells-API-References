---
title: ThreadedCommentAuthorCollection.CurrentPerson
second_title: Aspose.Cells for .NET API Reference
description: ThreadedCommentAuthorCollection property. Gets and sets the current user
type: docs
url: /net/aspose.cells/threadedcommentauthorcollection/currentperson/
---
## ThreadedCommentAuthorCollection.CurrentPerson property

Gets and sets the current user.

```csharp
public ThreadedCommentAuthor CurrentPerson { get; set; }
```

### Examples

```csharp
// Called: authors.CurrentPerson = authors[0];
[Test]
        public void Property_CurrentPerson()
        {
            Workbook workbook = new Workbook();
            ThreadedCommentAuthorCollection authors = workbook.Worksheets.ThreadedCommentAuthors;
            authors.Add("Aspose", "S::johnson.shi@asposenj.onmicrosoft.com::bd07c1a8-5f37-4ecf-bd20-1f831c9015ce", "AD");
            authors.CurrentPerson = authors[0];


            CommentCollection comments = workbook.Worksheets[0].Comments;
            comments.AddThreadedComment("B3", "Test1", null);
            comments.AddThreadedComment("B3", "Test2", null);
            comments.AddThreadedComment("B3", "Test3", null);
            workbook.Worksheets.Add();
            comments = workbook.Worksheets[1].Comments;
            comments.AddThreadedComment("B3", "Test11", null);
            comments.AddThreadedComment("B3", "Test12", null);
            comments.AddThreadedComment("B3", "Test13", null);
            workbook.Save(Constants.destPath + "CELLSNET46656_002.xlsx");
        }
```

### See Also

* class [ThreadedCommentAuthor](../../threadedcommentauthor/)
* class [ThreadedCommentAuthorCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


