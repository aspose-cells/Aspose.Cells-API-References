---
title: Shape.GetActualBox
second_title: Aspose.Cells for .NET API Reference
description: Shape method. Get the actual position and size of the shape after applying rotation flip etc
type: docs
url: /net/aspose.cells.drawing/shape/getactualbox/
---
## Shape.GetActualBox method

Get the actual position and size of the shape (after applying rotation, flip, etc.)

```csharp
public float[] GetActualBox()
```

### Return Value

Return the position and size in the order of x, y, w, h

### Remarks

Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.

### Examples

```csharp
// Called: float[] box = rect.GetActualBox();
[Test]
        public void Method_GetActualBox()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET-55913.xlsx&quot;);
            ShapeCollection shapes = wb.Worksheets[0].Shapes;

            Shape rect = shapes[&quot;Rectangle 1&quot;];
            rect.AddHyperlink(&quot;www.aspose.com&quot;);
            Assert.AreEqual(rect.Hyperlink.Address, &quot;www.aspose.com&quot;);

            rect.RemoveHyperlink();
            Assert.AreEqual(null, rect.Hyperlink);

            rect.SetInputRange(&quot;=A2&quot;, false, true);
            String inputRange = rect.GetInputRange(false, true);
            Assert.AreEqual(&quot;A2&quot;, inputRange);
            Assert.AreEqual(&quot;A2&quot;, rect.InputRange);

            float[] box = rect.GetActualBox();
            Assert.AreEqual(4, (int)box[0]);
            Assert.AreEqual(10, (int)box[1]);
            Assert.AreEqual(110, (int)box[2]);
            Assert.AreEqual(92, (int)box[3]);

            rect.SetLinkedCell(&quot;=A3&quot;, false, true);
            string linkCell = rect.GetLinkedCell(false, true);
            Assert.AreEqual(&quot;A3&quot;, linkCell);
            Assert.AreEqual(&quot;A3&quot;, rect.LinkedCell);

            CellArea shapesArea = CellArea.CreateCellArea(&quot;C5&quot;, &quot;H20&quot;);
            shapes.CopyInRange(shapes, shapesArea, 5, 12, false);
            Assert.AreEqual(8, shapes.Count);

            CellArea commentsArea = CellArea.CreateCellArea(&quot;C5&quot;, &quot;G10&quot;);
            shapes.CopyCommentsInRange(shapes, commentsArea, 5, 12);

            Assert.AreEqual(12, shapes.Count);

            shapes.DeleteInRange(shapesArea);
            Assert.AreEqual(10, shapes.Count);
        }
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


