---
title: GlowEffect.Transparency
second_title: Aspose.Cells for .NET API Reference
description: GlowEffect property. Gets and sets the degree of transparency of the glow effect. Range from 0.0 opaque to 1.0 clear
type: docs
url: /net/aspose.cells.drawing/gloweffect/transparency/
---
## GlowEffect.Transparency property

Gets and sets the degree of transparency of the glow effect. Range from 0.0 (opaque) to 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: shape.Glow.Transparency = 0.6;
public void GlowEffect_Property_Transparency()
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

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


