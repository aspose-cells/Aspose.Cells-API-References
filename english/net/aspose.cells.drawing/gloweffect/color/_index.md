---
title: GlowEffect.Color
second_title: Aspose.Cells for .NET API Reference
description: GlowEffect property. Gets the color of the glow effect
type: docs
url: /net/aspose.cells.drawing/gloweffect/color/
---
## GlowEffect.Color property

Gets the color of the glow effect.

```csharp
public CellsColor Color { get; set; }
```

### Examples

```csharp
// Called: CellsColor cColor = shape.Glow.Color;
public void GlowEffect_Property_Color()
{
    Workbook wb1 = new Workbook(Constants.sourcePath + "example.xlsx");// Please use both samples

    Shape shape = wb1.Worksheets[0].Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 0, 0, 100, 100);
    shape.Glow.Size = 8;
    shape.Glow.Transparency = 0.6;
    CellsColor cColor = shape.Glow.Color;
    cColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

    wb1.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


