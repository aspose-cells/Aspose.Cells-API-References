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
// Called: glowEffect.Transparency = 0.5;
public static void Property_Transparency()
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

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


