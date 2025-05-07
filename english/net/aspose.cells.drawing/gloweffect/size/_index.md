---
title: GlowEffect.Size
second_title: Aspose.Cells for .NET API Reference
description: GlowEffect property. Gets and sets the radius of the glow in unit of points
type: docs
url: /net/aspose.cells.drawing/gloweffect/size/
---
## GlowEffect.Size property

Gets and sets the radius of the glow, in unit of points.

```csharp
public double Size { get; set; }
```

### Examples

```csharp
// Called: shape.Glow.Size = 8;
[Test]
        public void Property_Size()
        {
            Workbook wb1 = new Workbook(Constants.sourcePath + "CellsNet43903.xlsx");// Please use both samples

            Shape shape = wb1.Worksheets[0].Shapes.AddAutoShape(AutoShapeType.RoundedRectangle, 0, 0, 0, 0, 100, 100);
            shape.Glow.Size = 8;
            shape.Glow.Transparency = 0.6;
            CellsColor cColor = shape.Glow.Color;
            cColor.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);

            wb1.Save(Constants.destPath + "CellsNet43903.xlsx");
        }
```

### See Also

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


