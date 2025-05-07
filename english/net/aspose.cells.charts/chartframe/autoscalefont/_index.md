---
title: ChartFrame.AutoScaleFont
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. True if the text in the object changes font size when the object size changes. The default value is True
type: docs
url: /net/aspose.cells.charts/chartframe/autoscalefont/
---
## ChartFrame.AutoScaleFont property

True if the text in the object changes font size when the object size changes. The default value is True.

```csharp
public virtual bool AutoScaleFont { get; set; }
```

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + ".AutoScaleFont");
public static void Property_AutoScaleFont(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + ".Position");
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + ".ShapeProperties.ShadowEffect.PresetType");
            CellsColorTest.Property_AutoScaleFont(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + ".ShapeProperties.ShadowEffect.Color");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + ".ShapeProperties.ShadowEffect.Transparency");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + ".ShapeProperties.ShadowEffect.Size");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + ".ShapeProperties.ShadowEffect.Blur");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + ".ShapeProperties.ShadowEffect.Angle");
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + ".ShapeProperties.ShadowEffect.Distance");


            //===================compare patterns===========//
            LineTest.Property_AutoScaleFont(legendSrc.Border, legendDest.Border, info + ".Border");
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + ".Shadow");
            AreaTest.Property_AutoScaleFont(legendSrc.Area, legendDest.Area, info + ".Area");
            //===================compare font==============//
            FontTest.Property_AutoScaleFont(legendSrc.TextFont, legendDest.TextFont, info + ".TextFont");
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + ".AutoScaleFont");
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + ".Background");
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + ".Height");
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + ".Width");
            LegendEntriesTest.Property_AutoScaleFont(legendSrc.LegendEntries, legendDest.LegendEntries, info + ".LegendEntries");           
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


