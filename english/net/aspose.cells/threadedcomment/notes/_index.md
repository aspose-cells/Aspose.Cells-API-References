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
// Called: Assert.AreEqual(comments[1].Notes, &amp;quot;2222222222222222222222222222222222222\n&amp;quot;);
[Test]
        public void Property_Notes()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET46656.xlsx&quot;);
            Assert.AreEqual(1, workbook.Worksheets.ThreadedCommentAuthors.Count);
            ThreadedCommentCollection comments = workbook.Worksheets[0].Comments.GetThreadedComments(4, 1);
            Assert.AreEqual(3, comments.Count);
            Assert.AreEqual(comments[0].Notes, &quot;11111111111111111111111111111111111\n&quot;);
            Assert.AreEqual(comments[1].Notes, &quot;2222222222222222222222222222222222222\n&quot;);
            Assert.AreEqual(comments[2].Notes, &quot;33333333333333333333333333333333333333\n&quot;);
            workbook.Save(Constants.destPath + &quot;CELLSNET46656.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET46656.xlsx&quot;);
            Assert.AreEqual(1, workbook.Worksheets.ThreadedCommentAuthors.Count);
            comments = workbook.Worksheets[0].Comments.GetThreadedComments(&quot;B5&quot;);
            Assert.AreEqual(3, comments.Count);
            Assert.AreEqual(comments[0].Notes, &quot;11111111111111111111111111111111111\n&quot;);
            Assert.AreEqual(comments[1].Notes, &quot;2222222222222222222222222222222222222\n&quot;);
            Assert.AreEqual(comments[2].Notes, &quot;33333333333333333333333333333333333333\n&quot;);
        }
```

### See Also

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


