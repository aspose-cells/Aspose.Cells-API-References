---
title: ThreadedComment.Notes
second_title: Aspose.Cells for .NET API Reference
description: ThreadedComment property. Gets and sets the text of the comment
type: docs
url: /net/aspose.cells/threadedcomment/notes/
---
## ThreadedComment.Notes property

Gets and sets the text of the comment.

```csharp
public string Notes { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(comments[1].Notes, "2222222222222222222222222222222222222\n");
public void ThreadedComment_Property_Notes()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    Assert.AreEqual(1, workbook.Worksheets.ThreadedCommentAuthors.Count);
    ThreadedCommentCollection comments = workbook.Worksheets[0].Comments.GetThreadedComments(4, 1);
    Assert.AreEqual(3, comments.Count);
    Assert.AreEqual(comments[0].Notes, "11111111111111111111111111111111111\n");
    Assert.AreEqual(comments[1].Notes, "2222222222222222222222222222222222222\n");
    Assert.AreEqual(comments[2].Notes, "33333333333333333333333333333333333333\n");
    workbook.Save(Constants.destPath + "example.xlsx");
    workbook = new Workbook(Constants.destPath + "example.xlsx");
    Assert.AreEqual(1, workbook.Worksheets.ThreadedCommentAuthors.Count);
    comments = workbook.Worksheets[0].Comments.GetThreadedComments("B5");
    Assert.AreEqual(3, comments.Count);
    Assert.AreEqual(comments[0].Notes, "11111111111111111111111111111111111\n");
    Assert.AreEqual(comments[1].Notes, "2222222222222222222222222222222222222\n");
    Assert.AreEqual(comments[2].Notes, "33333333333333333333333333333333333333\n");
}
```

### See Also

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


