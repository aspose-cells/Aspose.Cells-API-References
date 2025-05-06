---
title: ShadowEffect.Distance
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the distance of the shadow. Range from 0 to 200 points
type: docs
url: /net/aspose.cells.drawing/shadoweffect/distance/
---
## ShadowEffect.Distance property

Gets and sets the distance of the shadow. Range from 0 to 200 points.

```csharp
public double Distance { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Distance, shapeProDest.ShadowEffect.Distance, info + &amp;quot;.ShadowEffect.Distance&amp;quot;);
public static void Property_Distance(ShapePropertyCollection shapeProSrc, ShapePropertyCollection shapeProDest, string info)
        {
            //====================Shadow================//
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.PresetType, shapeProDest.ShadowEffect.PresetType, info + &quot;.ShadowEffect.PresetType&quot;);
            CellsColorTest.Property_Distance(shapeProSrc.ShadowEffect.Color, shapeProDest.ShadowEffect.Color, info + &quot;.ShadowEffect.Color&quot;);
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Transparency, shapeProDest.ShadowEffect.Transparency, info + &quot;.ShadowEffect.Transparency&quot;);
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Size, shapeProDest.ShadowEffect.Size, info + &quot;.ShadowEffect.Size&quot;);
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Blur, shapeProDest.ShadowEffect.Blur, info + &quot;.ShadowEffect.Blur&quot;);
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Angle, shapeProDest.ShadowEffect.Angle, info + &quot;.ShadowEffect.Angle&quot;);
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Distance, shapeProDest.ShadowEffect.Distance, info + &quot;.ShadowEffect.Distance&quot;);
            //====================3-D Format===============//
            AssertHelper.AreEqual(shapeProSrc.Format3D.TopBevel, shapeProDest.Format3D.TopBevel, info + &quot;.Format3D.TopBevel&quot;);
            //shapeProSrc.GlowEffect.Transparency
            //Surface
            AssertHelper.AreEqual(shapeProSrc.Format3D.SurfaceLightingType, shapeProDest.Format3D.SurfaceLightingType, info + &quot;.Format3D.SurfaceLightingType&quot;);
            AssertHelper.AreEqual(shapeProSrc.Format3D.SurfaceMaterialType, shapeProDest.Format3D.SurfaceMaterialType, info + &quot;.Format3D.SurfaceMaterialType&quot;);
            AssertHelper.AreEqual(shapeProSrc.Format3D.LightingAngle, shapeProDest.Format3D.LightingAngle, info + &quot;.Format3D.LightingAngle&quot;);
        }
```

### See Also

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


