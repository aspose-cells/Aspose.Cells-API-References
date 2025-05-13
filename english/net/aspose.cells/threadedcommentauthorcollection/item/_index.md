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
// Called: authors.CurrentPerson = authors[0];
public void ThreadedCommentAuthorCollection_Property_Item()
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
    workbook.Save(Constants.destPath + "example.xlsx");
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


