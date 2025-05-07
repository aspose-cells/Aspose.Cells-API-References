---
title: SolidFill.Color
second_title: Aspose.Cells for .NET API Reference
description: SolidFill property. Gets or sets the Color
type: docs
url: /net/aspose.cells.drawing/solidfill/color/
---
## SolidFill.Color property

Gets or sets the Color.

```csharp
public Color Color { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(Color.FromArgb(0xbfbfbf), workbok.Worksheets[0].Shapes[0].Fill.SolidFill.Color);
[Test]
        public void Property_Color()
        {
            Workbook workbok = new Workbook(Constants.sourcePath + "CELLSJAVA41364.ods");
            AssertHelper.AreEqual(Color.FromArgb(0xbfbfbf), workbok.Worksheets[0].Shapes[0].Fill.SolidFill.Color);
        }
```

### See Also

* class [SolidFill](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


