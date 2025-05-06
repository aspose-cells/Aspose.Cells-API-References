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
// Called: AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + &amp;quot;.ShapeProperties.ShadowEffect.Size&amp;quot;);
public static void Property_ShadowEffect(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + &quot;.Position&quot;);
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + &quot;.ShapeProperties.ShadowEffect.PresetType&quot;);
            CellsColorTest.Property_ShadowEffect(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + &quot;.ShapeProperties.ShadowEffect.Color&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + &quot;.ShapeProperties.ShadowEffect.Transparency&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + &quot;.ShapeProperties.ShadowEffect.Size&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + &quot;.ShapeProperties.ShadowEffect.Blur&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + &quot;.ShapeProperties.ShadowEffect.Angle&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + &quot;.ShapeProperties.ShadowEffect.Distance&quot;);


            //===================compare patterns===========//
            LineTest.Property_ShadowEffect(legendSrc.Border, legendDest.Border, info + &quot;.Border&quot;);
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + &quot;.Shadow&quot;);
            AreaTest.Property_ShadowEffect(legendSrc.Area, legendDest.Area, info + &quot;.Area&quot;);
            //===================compare font==============//
            FontTest.Property_ShadowEffect(legendSrc.TextFont, legendDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + &quot;.Background&quot;);
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + &quot;.Width&quot;);
            LegendEntriesTest.Property_ShadowEffect(legendSrc.LegendEntries, legendDest.LegendEntries, info + &quot;.LegendEntries&quot;);           
        }
```

### See Also

* class [ShadowEffect](../../shadoweffect/)
* class [ShapePropertyCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


