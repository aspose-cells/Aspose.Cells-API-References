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
// Called: AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + ".ShapeProperties.ShadowEffect.Distance");
public static void ShadowEffect_Property_Distance(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + ".Position");
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + ".ShapeProperties.ShadowEffect.PresetType");
            CellsColorTest.ShadowEffect_Property_Distance(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + ".ShapeProperties.ShadowEffect.Color");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + ".ShapeProperties.ShadowEffect.Transparency");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + ".ShapeProperties.ShadowEffect.Size");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + ".ShapeProperties.ShadowEffect.Blur");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + ".ShapeProperties.ShadowEffect.Angle");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + ".ShapeProperties.ShadowEffect.Distance");


            //===================compare patterns===========//
            LineTest.ShadowEffect_Property_Distance(legendSrc.Border, legendDest.Border, info + ".Border");
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + ".Shadow");
            AreaTest.ShadowEffect_Property_Distance(legendSrc.Area, legendDest.Area, info + ".Area");
            //===================compare font==============//
            FontTest.ShadowEffect_Property_Distance(legendSrc.TextFont, legendDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + ".Background");
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + ".Height");
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + ".Width");
            LegendEntriesTest.ShadowEffect_Property_Distance(legendSrc.LegendEntries, legendDest.LegendEntries, info + ".LegendEntries");           
        }
```

### See Also

* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


