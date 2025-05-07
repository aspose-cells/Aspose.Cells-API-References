---
title: ShadowEffect.Blur
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the blur of the shadow. Range from 0 to 100 points
type: docs
url: /net/aspose.cells.drawing/shadoweffect/blur/
---
## ShadowEffect.Blur property

Gets and sets the blur of the shadow. Range from 0 to 100 points.

```csharp
public double Blur { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Blur, shapeProDest.ShadowEffect.Blur, info + ".ShadowEffect.Blur");
public static void Property_Blur(ShapePropertyCollection shapeProSrc, ShapePropertyCollection shapeProDest, string info)
        {
            //====================Shadow================//
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.PresetType, shapeProDest.ShadowEffect.PresetType, info + ".ShadowEffect.PresetType");
            CellsColorTest.Property_Blur(shapeProSrc.ShadowEffect.Color, shapeProDest.ShadowEffect.Color, info + ".ShadowEffect.Color");
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Transparency, shapeProDest.ShadowEffect.Transparency, info + ".ShadowEffect.Transparency");
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Size, shapeProDest.ShadowEffect.Size, info + ".ShadowEffect.Size");
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Blur, shapeProDest.ShadowEffect.Blur, info + ".ShadowEffect.Blur");
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Angle, shapeProDest.ShadowEffect.Angle, info + ".ShadowEffect.Angle");
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Distance, shapeProDest.ShadowEffect.Distance, info + ".ShadowEffect.Distance");
            //====================3-D Format===============//
            AssertHelper.AreEqual(shapeProSrc.Format3D.TopBevel, shapeProDest.Format3D.TopBevel, info + ".Format3D.TopBevel");
            //shapeProSrc.GlowEffect.Transparency
            //Surface
            AssertHelper.AreEqual(shapeProSrc.Format3D.SurfaceLightingType, shapeProDest.Format3D.SurfaceLightingType, info + ".Format3D.SurfaceLightingType");
            AssertHelper.AreEqual(shapeProSrc.Format3D.SurfaceMaterialType, shapeProDest.Format3D.SurfaceMaterialType, info + ".Format3D.SurfaceMaterialType");
            AssertHelper.AreEqual(shapeProSrc.Format3D.LightingAngle, shapeProDest.Format3D.LightingAngle, info + ".Format3D.LightingAngle");
        }
```

### See Also

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


