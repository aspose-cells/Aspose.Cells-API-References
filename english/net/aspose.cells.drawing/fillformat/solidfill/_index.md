---
title: FillFormat.SolidFill
second_title: Aspose.Cells for .NET API Reference
description: FillFormat property. Gets SolidFill object
type: docs
url: /net/aspose.cells.drawing/fillformat/solidfill/
---
## FillFormat.SolidFill property

Gets `SolidFill` object.

```csharp
public SolidFill SolidFill { get; }
```

### Examples

```csharp
// Called: Color color = shape.Fill.SolidFill.Color;
public void FillFormat_Property_SolidFill()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");

    Shape shape = workbook.Worksheets[0].Shapes[0];
    Color color = shape.Fill.SolidFill.Color;
    Assert.AreEqual(135, color.R);
    Assert.AreEqual(222, color.G);
    Assert.AreEqual(255, color.B);
}
```

### See Also

* class [SolidFill](../../solidfill/)
* class [FillFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


