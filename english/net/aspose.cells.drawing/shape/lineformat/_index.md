---
title: Shape.LineFormat
second_title: Aspose.Cells for .NET API Reference
description: Shape property. Returns a MsoLineFormat object that contains line formatting properties for the specified shape
type: docs
url: /net/aspose.cells.drawing/shape/lineformat/
---
## Shape.LineFormat property

Returns a MsoLineFormat object that contains line formatting properties for the specified shape.

```csharp
[Obsolete("Use Shape.Line property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public MsoLineFormat LineFormat { get; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: Assert.AreEqual(shapes[0].LineFormat.Weight, 3.25);
[Test]
        public void Property_LineFormat()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsJava40399.xlsx");
            ShapeCollection shapes = workbook.Worksheets[0].Shapes;
            Assert.AreEqual(shapes[0].LineFormat.Weight, 3.25);
            Assert.AreEqual(shapes[1].LineFormat.Weight, 3.25);
        }
```

### See Also

* class [MsoLineFormat](../../msolineformat/)
* class [Shape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


