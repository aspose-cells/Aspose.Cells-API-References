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
public void ScrollBar_Property_IsHorizontal()
{
    Workbook workbook = new Workbook(Constants.sourcePath +"example.xls");
    ShapeCollection shapes = workbook.Worksheets[0].Shapes;
    Assert.AreEqual("Check Box 3", shapes[2].Text);
    Assert.AreEqual("Group Box 7", shapes[6].Text);
    Assert.IsTrue(((ScrollBar)shapes[shapes.Count - 1]).IsHorizontal);
    workbook.Save(Constants.destPath + "example.xls");

}
```

### See Also

* class [ScrollBar](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


