---
title: Shape.CreateId
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Gets and sets create id for this shape
type: docs
url: /net/aspose.cells.drawing/shape/createid/
---
## Shape.CreateId property

Gets and sets create id for this shape.

```csharp
public Guid CreateId { get; set; }
```

### Examples

```csharp
// Called: s.CreateId = g;
[Test]
        public void Property_CreateId()
        {
            Workbook workbook = new Workbook();
            RectangleShape s = workbook.Worksheets[0].Shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            Guid g = Guid.NewGuid();
            s.CreateId = g;
            workbook.Save(Constants.destPath + &quot;CellsNet51226.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet51226.xlsx&quot;);
            Shape s0 = workbook.Worksheets[0].Shapes[0];
            Assert.AreEqual(s0.CreateId, g);

        }
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


