---
title: Format3D.TopBevel
second_title: Aspose.Cells for .NET API Reference
description: Format3D property. Gets the Bevel object that holds the properties associated with defining a bevel on the top or front face of a shape
type: docs
url: /net/aspose.cells.drawing/format3d/topbevel/
---
## Format3D.TopBevel property

Gets the [`Bevel`](../../bevel/) object that holds the properties associated with defining a bevel on the top or front face of a shape.

```csharp
public Bevel TopBevel { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(shapeProSrc.Format3D.TopBevel, shapeProDest.Format3D.TopBevel, info + ".Format3D.TopBevel");
public static void Property_TopBevel(ShapePropertyCollection shapeProSrc, ShapePropertyCollection shapeProDest, string info)
        {
            //====================Shadow================//
            AssertHelper.AreEqual(shapeProSrc.ShadowEffect.PresetType, shapeProDest.ShadowEffect.PresetType, info + ".ShadowEffect.PresetType");
            CellsColorTest.Property_TopBevel(shapeProSrc.ShadowEffect.Color, shapeProDest.ShadowEffect.Color, info + ".ShadowEffect.Color");
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

* class [Bevel](../../bevel/)
* class [Format3D](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


