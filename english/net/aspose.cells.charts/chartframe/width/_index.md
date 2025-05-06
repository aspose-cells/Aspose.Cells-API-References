---
title: ChartFrame.Width
second_title: Aspose.Cells for .NET API Reference
description: ChartFrame property. Gets or sets the width of frame in units of 1/4000 of the chart area
type: docs
url: /net/aspose.cells.charts/chartframe/width/
---
## ChartFrame.Width property

Gets or sets the width of frame in units of 1/4000 of the chart area.

```csharp
[Obsolete("Use ChartFrame.WidthRatioToChart property, instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public virtual int Width { get; set; }
```

### Remarks

How to convert units of 1/4000 to pixels? Width In Pixels = Width * Chart.ChartObject.Height / 4000d;

NOTE: This member is now obsolete. Please use ChartFrame.WidthRatioToChart property, instead. Width = WidthRatioToChart * 4000; This property will be removed 12 months later since February 2025. Aspose apologizes for any inconvenience you may have experienced.

### Examples

```csharp
// Called: AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + &amp;quot;.Width&amp;quot;);
public static void Property_Width(Legend legendSrc, Legend legendDest, string info)
        {
            if (AssertHelper.checkNull(legendSrc, legendDest, info))
            {
                return;
            }
            //==============Legend Options=================//
            AssertHelper.AreEqual(legendSrc.Position, legendDest.Position, info + &quot;.Position&quot;);
            //=====================Shadow Option=============//
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.PresetType, legendDest.ShapeProperties.ShadowEffect.PresetType, info + &quot;.ShapeProperties.ShadowEffect.PresetType&quot;);
            CellsColorTest.Property_Width(legendSrc.ShapeProperties.ShadowEffect.Color, legendDest.ShapeProperties.ShadowEffect.Color, info + &quot;.ShapeProperties.ShadowEffect.Color&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Transparency, legendDest.ShapeProperties.ShadowEffect.Transparency, info + &quot;.ShapeProperties.ShadowEffect.Transparency&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Size, legendDest.ShapeProperties.ShadowEffect.Size, info + &quot;.ShapeProperties.ShadowEffect.Size&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Blur, legendDest.ShapeProperties.ShadowEffect.Blur, info + &quot;.ShapeProperties.ShadowEffect.Blur&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Angle, legendDest.ShapeProperties.ShadowEffect.Angle, info + &quot;.ShapeProperties.ShadowEffect.Angle&quot;);
            AssertHelper.AreEqual(legendSrc.ShapeProperties.ShadowEffect.Distance, legendDest.ShapeProperties.ShadowEffect.Distance, info + &quot;.ShapeProperties.ShadowEffect.Distance&quot;);


            //===================compare patterns===========//
            LineTest.Property_Width(legendSrc.Border, legendDest.Border, info + &quot;.Border&quot;);
            AssertHelper.AreEqual(legendSrc.Shadow, legendDest.Shadow, info + &quot;.Shadow&quot;);
            AreaTest.Property_Width(legendSrc.Area, legendDest.Area, info + &quot;.Area&quot;);
            //===================compare font==============//
            FontTest.Property_Width(legendSrc.TextFont, legendDest.TextFont, info + &quot;.TextFont&quot;);
            AssertHelper.AreEqual(legendSrc.AutoScaleFont, legendDest.AutoScaleFont, info + &quot;.AutoScaleFont&quot;);
            AssertHelper.AreEqual(legendSrc.BackgroundMode, legendDest.BackgroundMode, info + &quot;.Background&quot;);
            //===================compare placement=========//
           
            //==================compare other==============//
            AssertHelper.AreEqual(legendSrc.Height, legendDest.Height, info + &quot;.Height&quot;);
            AssertHelper.AreEqual(legendSrc.Width, legendDest.Width, info + &quot;.Width&quot;);
            LegendEntriesTest.Property_Width(legendSrc.LegendEntries, legendDest.LegendEntries, info + &quot;.LegendEntries&quot;);           
        }
```

### See Also

* class [ChartFrame](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


