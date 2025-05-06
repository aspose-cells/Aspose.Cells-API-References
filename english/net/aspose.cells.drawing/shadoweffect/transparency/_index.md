---
title: ShadowEffect.Transparency
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the degree of transparency of the shadow. Range from 0.0 opaque to 1.0 clear
type: docs
url: /net/aspose.cells.drawing/shadoweffect/transparency/
---
## ShadowEffect.Transparency property

Gets and sets the degree of transparency of the shadow. Range from 0.0 (opaque) to 1.0 (clear).

```csharp
public double Transparency { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(shapeProSrc.ShadowEffect.Transparency, shapeProDest.ShadowEffect.Transparency, info + &amp;quot;.ShadowEffect.Transparency&amp;quot;);
public static void Property_Transparency(ShapePropertyCollection shapeProSrc, ShapePropertyCollection shapeProDest, string info)
        {
            //====================Shadow================//
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.PresetType, shapeProDest.ShadowEffect.PresetType, info + &quot;.ShadowEffect.PresetType&quot;);
            CellsColorTest.Property_Transparency(shapeProSrc.ShadowEffect.Color, shapeProDest.ShadowEffect.Color, info + &quot;.ShadowEffect.Color&quot;);
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


