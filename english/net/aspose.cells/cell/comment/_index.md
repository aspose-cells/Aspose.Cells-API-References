---
title: Cell.Comment
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets the comment of this cell
type: docs
url: /net/aspose.cells/cell/comment/
---
## Cell.Comment property

Gets the comment of this cell.

```csharp
public Comment Comment { get; }
```

### Remarks

If there is no comment applies to the cell, returns null.

### Examples

```csharp
// Called: comment = F4_Cell.Comment;
[Test]
        public void Property_Comment()
        {
            Workbook wb = new Workbook(Constants.sourcePath + @&quot;Numbers13\ExpTest\threadComment.xlsx&quot;);
#if APPLECHECK
            wb.Save(Constants.sourcePath + @&quot;Numbers13\ExpTest\threadComment_Ret.numbers&quot;);
#endif
            Workbook numbers = Util.ReSave(wb, SaveFormat.Numbers);
            Cells cells = numbers.Worksheets[0].Cells;
            //sheet1 A2
            Cell A2_Cell = cells[&quot;A2&quot;];
            Comment comment = A2_Cell.Comment;
            Assert.AreEqual(&quot;xinya zhu&quot;, comment.Author);
            Assert.AreEqual(&quot;xinya zhu:\n123&quot;, comment.Note);

            Cell F4_Cell = cells[&quot;F4&quot;];
            comment = F4_Cell.Comment;
            Assert.AreEqual(null, comment);
            Assert.AreEqual(&quot;asd&quot;, F4_Cell.StringValue);
            //sheet1 B3 D4
            //Read Threaded comment is not supported
            //To do ...
        }
```

### See Also

* class [Comment](../../comment/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


