---
title: Class ThreadedComment
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.ThreadedComment class. Represents the threaded comment
type: docs
url: /net/aspose.cells/threadedcomment/
---
## ThreadedComment class

Represents the threaded comment.

```csharp
public class ThreadedComment
```

## Properties

| Name | Description |
| --- | --- |
| [Author](../../aspose.cells/threadedcomment/author/) { get; set; } | Gets the author of the comment. |
| [Column](../../aspose.cells/threadedcomment/column/) { get; } | Gets the column index of the comment. |
| [CreatedTime](../../aspose.cells/threadedcomment/createdtime/) { get; set; } | Gets and sets the created time of this threaded comment. |
| [Notes](../../aspose.cells/threadedcomment/notes/) { get; set; } | Gets and sets the text of the comment. |
| [Row](../../aspose.cells/threadedcomment/row/) { get; } | Gets the row index of the comment. |

### Examples

```csharp
// Called: ThreadedComment tc = workbook.Worksheets[0].Comments[0].ThreadedComments[0];
[Test]
        public void Type_ThreadedComment()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;PYTHONJAVA-68.xlsx&quot;);
            ThreadedComment tc = workbook.Worksheets[0].Comments[0].ThreadedComments[0];
            Assert.AreEqual(DateTime.Now.Month, tc.CreatedTime.Month);
            workbook.Save(Constants.destPath + &quot;PYTHONJAVA-68.xlsx&quot;);
        }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


