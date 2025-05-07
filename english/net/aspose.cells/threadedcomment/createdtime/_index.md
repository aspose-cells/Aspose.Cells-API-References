---
title: ThreadedComment.CreatedTime
second_title: Aspose.Cells for .NET API Reference
description: ThreadedComment property. Gets and sets the created time of this threaded comment
type: docs
url: /net/aspose.cells/threadedcomment/createdtime/
---
## ThreadedComment.CreatedTime property

Gets and sets the created time of this threaded comment.

```csharp
public DateTime CreatedTime { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(DateTime.Now.Month, tc.CreatedTime.Month);
[Test]
        public void Property_CreatedTime()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "PYTHONJAVA-68.xlsx");
            ThreadedComment tc = workbook.Worksheets[0].Comments[0].ThreadedComments[0];
            Assert.AreEqual(DateTime.Now.Month, tc.CreatedTime.Month);
            workbook.Save(Constants.destPath + "PYTHONJAVA-68.xlsx");
        }
```

### See Also

* class [ThreadedComment](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


