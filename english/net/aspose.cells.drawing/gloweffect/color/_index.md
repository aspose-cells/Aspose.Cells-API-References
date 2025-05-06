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
// Called: glowEffect.Color = workbook.CreateCellsColor();
public static void Property_Color()
        {
            // Create a new workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Add an arc shape to the worksheet
            ArcShape arcShape = worksheet.Shapes.AddArc(2, 0, 2, 0, 130, 130);

            // Set the placement of the arc
            arcShape.Placement = PlacementType.FreeFloating;

            // Set the fill format
            arcShape.Fill.FillType = FillType.Solid;
            arcShape.Fill.SolidFill.Color = Color.Blue;

            // Set the line style
            arcShape.Line.CompoundType = MsoLineStyle.Single;
            arcShape.Line.Weight = 2;
            arcShape.Line.FillType = FillType.Solid;
            arcShape.Line.SolidFill.Color = Color.Red;
            arcShape.Line.DashStyle = MsoLineDashStyle.Solid;

            // Create a GlowEffect instance and set its properties
            GlowEffect glowEffect = arcShape.Glow;
            glowEffect.Color = workbook.CreateCellsColor();
            glowEffect.Color.Color = Color.Yellow;
            glowEffect.Radius = 10.0;
            glowEffect.Transparency = 0.5;

            // Save the workbook
            workbook.Save(&quot;GlowEffectExample.xlsx&quot;);
            workbook.Save(&quot;GlowEffectExample.pdf&quot;);
        }
```

### See Also

* class [CellsColor](../../../aspose.cells/cellscolor/)
* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


