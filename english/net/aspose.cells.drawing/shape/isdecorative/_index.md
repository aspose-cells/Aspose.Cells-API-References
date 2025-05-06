---
title: Shape.IsDecorative
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Indicates whether the object is decorative
type: docs
url: /net/aspose.cells.drawing/shape/isdecorative/
---
## Shape.IsDecorative property

Indicates whether the object is decorative.

```csharp
public bool IsDecorative { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].Shapes[0].IsDecorative);
[Test]
        public void Property_IsDecorative()
        {
            Workbook workbook = new Workbook();
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            shapes.AddRectangle(0, 0, 0, 0, 100, 100);
            shapes[0].IsDecorative = true;
            workbook.Save(Constants.destPath + &quot;CELLSNET56022.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET56022.xlsx&quot;);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].IsDecorative);
            workbook.Save(Constants.destPath + &quot;CELLSNET56022.xlsb&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET56022.xlsb&quot;);
            Assert.IsTrue(workbook.Worksheets[0].Shapes[0].IsDecorative);
        }
```

### See Also

* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


