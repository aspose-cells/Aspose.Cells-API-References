---
title: ShapeTextAlignment.IsLockedText
second_title: Aspose.Cells for .NET API Reference
description: ShapeTextAlignment property. Indicates whether the shape is locked when worksheet is protected
type: docs
url: /net/aspose.cells.drawing.texts/shapetextalignment/islockedtext/
---
## ShapeTextAlignment.IsLockedText property

Indicates whether the shape is locked when worksheet is protected.

```csharp
public bool IsLockedText { get; set; }
```

### Remarks

Only works when worksheet is protected.

### Examples

```csharp
// Called: Assert.IsTrue(tb.TextBody.TextAlignment.IsLockedText);
public void ShapeTextAlignment_Property_IsLockedText()
{
    Workbook w = new Workbook(Constants.sourcePath + "example.xls");
    Worksheet s = w.Worksheets[0];

    TextBox tb = s.Shapes.AddTextBox(3, 0, 7, 0, 30, 50);
    tb.Text = "TextBox002";
    Assert.IsTrue(tb.TextBody.TextAlignment.IsLockedText);
    w.Save(Constants.destPath + "example.xls");
    Workbook workbook = new Workbook(Constants.destPath + "example.xls");
    Shape shape = workbook.Worksheets[0].Shapes[1];
    Assert.IsTrue(shape.TextBody.TextAlignment.IsLockedText);
    Assert.IsTrue(tb.TextBody.TextAlignment.IsLockedText);
    workbook.Save(Constants.destPath + "example.xlsx");
     workbook = new Workbook(Constants.destPath + "example.xlsx");
     shape = workbook.Worksheets[0].Shapes[1];
    Assert.IsTrue(shape.TextBody.TextAlignment.IsLockedText);
}
```

### See Also

* class [ShapeTextAlignment](../)
* namespace [Aspose.Cells.Drawing.Texts](../../../aspose.cells.drawing.texts/)
* assembly [Aspose.Cells](../../../)


