---
title: GlowEffect.Radius
second_title: Aspose.Cells for .NET API Reference
description: GlowEffect property. Gets and sets the radius of the glow in unit of points
type: docs
url: /net/aspose.cells.drawing/gloweffect/radius/
---
## GlowEffect.Radius property

Gets and sets the radius of the glow, in unit of points.

```csharp
[Obsolete("Use GlowEffect.Size property instead.")]
public double Radius { get; set; }
```

### Remarks

NOTE: This member is now obsolete. Instead, please use GlowEffect.Size property. This property will be removed 6 months later since September 2016. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: glowEffect.Radius = 10.0;
public static void GlowEffect_Property_Radius()
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
            workbook.Save("GlowEffectExample.xlsx");
            workbook.Save("GlowEffectExample.pdf");
        }
```

### See Also

* class [GlowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


