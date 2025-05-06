---
title: ShadowEffect.PresetType
second_title: Aspose.Cells for .NET API Reference
description: ShadowEffect property. Gets and sets the preset shadow type of the shadow
type: docs
url: /net/aspose.cells.drawing/shadoweffect/presettype/
---
## ShadowEffect.PresetType property

Gets and sets the preset shadow type of the shadow.

```csharp
public PresetShadowType PresetType { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + &amp;quot;.ShapeProperties.ShadowEffect.PresetType&amp;quot;);
public static void Property_PresetType(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + &quot;.Position&quot;);
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + &quot;.ShapeProperties.ShadowEffect.PresetType&quot;);
            CellsColorTest.Property_PresetType(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + &quot;.ShapeProperties.ShadowEffect.Color&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + &quot;.ShapeProperties.ShadowEffect.Transparency&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + &quot;.ShapeProperties.ShadowEffect.Size&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + &quot;.ShapeProperties.ShadowEffect.Blur&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + &quot;.ShapeProperties.ShadowEffect.Angle&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + &quot;.ShapeProperties.ShadowEffect.Distance&quot;);


            //===================compare patterns===========//
            LineTest.Property_PresetType(legendSrc.Border, legendDest.Border, info + &quot;.Border&quot;);
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + &quot;.Shadow&quot;);
            AreaTest.Property_PresetType(legendSrc.Area, legendDest.Area, info + &quot;.Area&quot;);
            //===================compare font==============//
            FontTest.Property_PresetType(legendSrc.TextFont, legendDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + &quot;.Background&quot;);
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + &quot;.Width&quot;);
            LegendEntriesTest.Property_PresetType(legendSrc.LegendEntries, legendDest.LegendEntries, info + &quot;.LegendEntries&quot;);           
        }
```

### See Also

* enum [PresetShadowType](../../presetshadowtype/)
* class [ShadowEffect](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


