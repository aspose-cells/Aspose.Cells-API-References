---
title: ScrollBar.IsHorizontal
second_title: Aspose.Cells for .NET API Reference
description: ScrollBar property. Indicates whether this is a horizontal scroll bar
type: docs
url: /net/aspose.cells.drawing/scrollbar/ishorizontal/
---
## ScrollBar.IsHorizontal property

Indicates whether this is a horizontal scroll bar.

```csharp
public bool IsHorizontal { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(((ScrollBar)shapes[shapes.Count - 1]).IsHorizontal);
[Test]
        public void Property_IsHorizontal()
        {
            Workbook workbook = new Workbook(Constants.sourcePath +&quot;CellsNet48020.xls&quot;);
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            Assert.AreEqual(&quot;Check Box 3&quot;, shapes[2].Text);
            Assert.AreEqual(&quot;Group Box 7&quot;, shapes[6].Text);
            Assert.IsTrue(((ScrollBar)shapes[shapes.Count - 1]).IsHorizontal);
            workbook.Save(Constants.destPath + &quot;CellsNet48020.xls&quot;);

        }
```

### See Also

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


