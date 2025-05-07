---
title: ShapePropertyCollection.ShadowEffect
second_title: Aspose.Cells for .NET API Reference
description: ShapePropertyCollection property. Represents a ShadowEffect object that specifies shadow effect for the chart element or shape
type: docs
url: /net/aspose.cells.drawing/shapepropertycollection/shadoweffect/
---
## ShapePropertyCollection.ShadowEffect property

Represents a `ShadowEffect` object that specifies shadow effect for the chart element or shape.

```csharp
public ShadowEffect ShadowEffect { get; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + ".ShapeProperties.ShadowEffect.Transparency");
public static void Property_ShadowEffect(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + ".Position");
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + ".ShapeProperties.ShadowEffect.PresetType");
            CellsColorTest.Property_ShadowEffect(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + ".ShapeProperties.ShadowEffect.Color");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + ".ShapeProperties.ShadowEffect.Transparency");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + ".ShapeProperties.ShadowEffect.Size");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + ".ShapeProperties.ShadowEffect.Blur");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + ".ShapeProperties.ShadowEffect.Angle");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + ".ShapeProperties.ShadowEffect.Distance");


            //===================compare patterns===========//
            LineTest.Property_ShadowEffect(legendSrc.Border, legendDest.Border, info + ".Border");
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + ".Shadow");
            AreaTest.Property_ShadowEffect(legendSrc.Area, legendDest.Area, info + ".Area");
            //===================compare font==============//
            FontTest.Property_ShadowEffect(legendSrc.TextFont, legendDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + ".Background");
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + ".Height");
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + ".Width");
            LegendEntriesTest.Property_ShadowEffect(legendSrc.LegendEntries, legendDest.LegendEntries, info + ".LegendEntries");           
        }
```

### See Also

* class [ShadowEffect](../../shadoweffect/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


